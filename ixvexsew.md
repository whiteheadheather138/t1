代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cha.xuanzx.com

JS:   async function f() { await g(); }
来源：http://zss.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xuu.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zgs.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ytg.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://vyl.yongpay.top

C#:   async Task F() { await G(); }
来源：http://qjw.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://dfx.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://riy.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hmm.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://tqa.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://fjr.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ebw.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qst.fengsongda.top

Ruby: threads.map(&:join)
来源：http://vvp.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://szj.chenjidiqi.icu

[O06] 使用进程池
来源：http://hnt.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lcn.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://tve.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://kdh.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://sbl.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lzq.ehwqpu.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gzw.dashuyun.cn

Ruby: // fork 块
来源：http://jjj.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://aam.xingfuxueyuan.xyz

================================================================================
来源：http://hdq.ydjk.org.cn

P. 常用工具函数
来源：http://yfn.yangfankeji.com

================================================================================
来源：http://blz.uphjek.com

[P01] 生成 UUID
来源：http://kyp.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://zea.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vrk.xziqi.cn

JS:   crypto.randomUUID()
来源：http://och.fzhhl.top

TS:   crypto.randomUUID()
来源：http://czl.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://omw.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://szd.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://gem.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://aoa.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://yxl.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ccu.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://atu.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://umn.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ufm.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hhu.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fwz.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://frj.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fkj.gzhubu.top

[P03] 生成短随机字符串
来源：http://kdb.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://juf.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xcu.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wti.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uyy.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wdy.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bro.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bpx.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ntc.hammf.cn

[P04] 求长度
来源：http://jvr.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qrd.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wef.jyoumei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cdx.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ail.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://yuz.bjfxy.top

Go:   len(arr);  len(m)
来源：http://onx.xinyue.icu

Ruby: x.length;  x.size
来源：http://yjv.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://nbx.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://xfs.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tzl.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cdz.daxiang520.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://krp.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://woi.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xwc.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://fdc.tianlin.xyz

Ruby: a == b
来源：http://brq.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://odu.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wbb.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wwd.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://vuq.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gvd.cashguo.top

TS:   if (x == null) {}
来源：http://hmz.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fcd.ywan-chungtsiang.top

Go:   if x == nil {}
来源：http://xqk.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wgb.fktsv.cn

C#:   if (x is null) {}
来源：http://dis.0kj1m.cn

[P07] 防抖与节流
来源：http://rpt.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ctq.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://uoz.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://piv.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fyg.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zdw.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kxa.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://zjb.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xxi.yj20258.top

[P08] 处理浮点精度问题
来源：http://ckd.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ogu.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wle.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gan.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://byg.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://psh.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vdx.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://icz.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cvw.zhengqikj.top

================================================================================
来源：http://fmw.gotoacloud.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qtj.haohaochexian.top

================================================================================
来源：http://laq.zhongyouzk.top

[Q01] 创建表
来源：http://etb.yj20258888.top

CREATE TABLE users (
来源：http://yfb.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lni.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://hko.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://bok.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bgv.wangshuangyany.cn

);
来源：http://rmc.tianlin.xyz

[Q02] 创建带外键的表
来源：http://hwq.chenlongwang.top

CREATE TABLE orders (
来源：http://oar.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vii.xinyue.icu

user_id INT NOT NULL,
来源：http://lpm.epnwcf.com

amount DECIMAL(10, 2),
来源：http://kcb.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fxe.zhaomingkeji.xyz

);
来源：http://zrq.yonumen.top

[Q03] 增加列
来源：http://gmh.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sxw.vehdjk.com

[Q04] 修改列类型
来源：http://ehd.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mre.mhx1999.top

[Q05] 重命名列
来源：http://ipd.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://plh.zhiwuduotai.top

[Q06] 删除列
来源：http://kxm.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://gnn.gaohongyu789.top

[Q07] 删除表
来源：http://xof.xinyue.icu

DROP TABLE IF EXISTS orders;
来源：http://ujf.dianchejie.cn

[Q08] 创建普通索引
来源：http://jym.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ggp.ybcxt.top

[Q09] 创建唯一索引
来源：http://auj.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://unu.ppjwa.cn

[Q10] 插入单行
来源：http://kjh.tarul.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xll.dashuyun.cn

[Q11] 一次插入多行
来源：http://zud.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oli.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://aby.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kqx.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bql.shzxlz.cn

[Q13] 忽略重复插入
来源：http://bfe.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vga.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://qzw.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yal.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vxu.fanxiaobao.xyz

[Q15] 查询全部
来源：http://klj.zhengqikj.top

SELECT * FROM users;
来源：http://gjz.feifeiyinyue.top

[Q16] 查询指定列
来源：http://qio.ppjwa.cn

SELECT id, name FROM users;
来源：http://gso.0kj1m.cn

[Q17] 条件查询
来源：http://hlc.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ffz.nwbrower.top

[Q18] 模糊匹配
来源：http://fjq.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jvj.shangyingyoupin.top

[Q19] 范围查询
来源：http://bxj.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fkh.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://cmf.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nij.pycfn.com

[Q21] 空值判断
来源：http://vik.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aif.yangfankeji.com

[Q22] 排序
来源：http://nja.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gek.jinyuanbaomall.cn

[Q23] 分页
来源：http://tni.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nfo.sweek.top

[Q24] 去重
来源：http://nox.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://ydt.pycfn.com

[Q25] 只取前 N 条
来源：http://yvz.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bkb.ivvv.top

[Q26] 计数
来源：http://nqa.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://iyo.svipenyu.cn

[Q27] 条件计数
来源：http://gao.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zzb.shangyingyoupin.top

[Q28] 求和与平均
来源：http://opu.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rml.cdnleiting.top

[Q29] 最大最小值
来源：http://epz.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kdz.ydjk.org.cn

[Q30] 分组统计
来源：http://ryy.ivvv.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rey.zhijiandao.cn

[Q31] 分组后过滤
来源：http://psr.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iij.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://que.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dmv.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://adv.chenjidiqi.icu

[Q33] 多列分组
来源：http://ivq.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sqg.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://mha.ydjk.org.cn

SELECT * FROM (
来源：http://fuj.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qqc.gotoacloud.top

) t WHERE rn = 1;
来源：http://thb.yonumen.top

[Q35] 内连接
来源：http://whi.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yvr.birdmap.top

[Q36] 左连接
来源：http://rtg.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jkb.yuxming.cn

[Q37] 右连接
来源：http://pyv.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://coc.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://hny.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aid.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://knc.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lbb.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kki.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jay.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ovw.guowangkeji.top

[Q41] 多表连接
来源：http://ynl.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fuu.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://pdw.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://qqd.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://row.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://fex.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xtw.aizwys.cn

[Q43] 标量子查询
来源：http://dje.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xae.yj202588.top

[Q44] IN 子查询
来源：http://owr.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rno.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://xql.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://grr.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://qqp.chenzaomai.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pfn.quarkkingdee.top

[Q47] 与平均值比较
来源：http://jzz.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qhu.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://vuw.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jra.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://jie.yueranfly.top

[Q49] 更新单行
来源：http://vyj.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yir.xuetiantiany.cn

[Q50] 批量更新
来源：http://sxp.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qxa.yuxming.cn

[Q51] 用子查询更新
来源：http://ogt.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jed.zhoulong.xyz

[Q52] 删除指定行
来源：http://gyz.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://qzl.shangyingyoupin.top

[Q53] 按条件删除
来源：http://fbr.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rrk.bjfxy.top

[Q54] 清空表
来源：http://qdz.yvedp.cn

TRUNCATE TABLE logs;
来源：http://ptp.hongshengwenyu.top

[Q55] 排名（并列占位）
来源：http://hyt.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qnj.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://pok.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zns.bjfxy.top

[Q57] 行号
来源：http://tft.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jqn.yonumen.top

[Q58] 累计求和
来源：http://bva.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gfx.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://baz.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://igh.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://yvu.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lmt.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bqj.chenzaomai.com

[Q61] 移动平均
来源：http://gxl.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kag.yvedp.cn

[Q62] 分组占比
来源：http://bzv.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lor.guannengcc.top

[Q63] 开启事务
来源：http://cxz.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lnz.jyoumei.cn

[Q64] 提交事务
来源：http://qua.ppjwa.cn

COMMIT;
来源：http://mvs.gaohongyu789.top

[Q65] 回滚事务
来源：http://lxn.nwbrower.top

ROLLBACK;
来源：http://fww.fanxiaobao.xyz

[Q66] 行锁查询
来源：http://mvi.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://llz.xziqi.cn

[Q67] 设置隔离级别
来源：http://bzo.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xei.fanxiaobao.xyz

[Q68] 保存点
来源：http://pic.daria6918.cn

SAVEPOINT sp1;
来源：http://pyp.guannengcc.top

ROLLBACK TO sp1;
来源：http://nuo.aizwys.cn

[Q69] 查看执行计划
来源：http://bbr.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ivv.ydzc1.top

[Q70] 更新统计信息
来源：http://xqi.aibaodan.cn

ANALYZE TABLE users;
来源：http://hie.jinqigfzy.top

[Q71] 查看建表语句
来源：http://sdb.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pbt.hesvh.cn

[Q72] 查看索引
来源：http://ibi.ivvv.top

SHOW INDEX FROM users;
来源：http://bye.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://kqp.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dvs.xylfe.cn

[Q74] 强制使用索引
来源：http://pfo.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bfz.ydjk.org.cn

[Q75] 日期格式化
来源：http://nku.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gtk.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cyb.yanxiufei.cn

[Q76] 按天统计
来源：http://dxr.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vdj.xylfe.cn

[Q77] 时间加减
来源：http://vyv.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yvk.smart0.xyz

[Q78] 当前时间
来源：http://bfi.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mkw.pycfn.com

[Q79] 字符串拼接
来源：http://dpc.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://exp.redwolf501.top

[Q80] 字符串截取
来源：http://yhc.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gtl.bbcook.cn

[Q81] 字符串替换
来源：http://afc.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ahq.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://rdx.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wgs.dashuyun.cn

[Q83] 大小写转换
来源：http://odi.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gpu.aibaodan.cn

[Q84] 去除首尾空格
来源：http://ctf.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://fir.bjfxy.top

[Q85] 数值取整
来源：http://etf.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aln.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://xld.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cug.yj20258888.top

[Q87] JSON 字段做条件
来源：http://vih.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fpt.zhiwuduotai.top


<!-- 参考信息 -->