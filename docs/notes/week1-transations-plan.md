# Week 1 Transactions Plan

1. Create the transaction domain model in src/BudgetTracker.Api/Features/Transactions/TransactionTypes.cs with required fields, validation attributes, and PostgreSQL-friendly column types.
2. Add TransactionDto and a MapToDto extension in the same file so API responses stay decoupled from EF entities.
3. Update src/BudgetTracker.Api/Infrastructure/BudgetTrackerContext.cs to register DbSet<Transaction> and add indexes for Date, UserId, and ImportedAt.
4. Complete Transaction model configuration in OnModelCreating, including primary key/default UUID generation and the UserId foreign key to ApplicationUser.Id.
5. Generate and apply an EF Core migration (AddTransactionEntity), then verify the Transactions table and indexes were created successfully.
