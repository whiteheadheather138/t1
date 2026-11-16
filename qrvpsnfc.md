代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://odz.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://xdc.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://ymu.yj20258.top

Py:   async def f():⏎    await g()
来源：http://vfg.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://drj.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://luv.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qfp.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mev.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kgd.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://qhf.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://tgy.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://yua.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://qxn.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qcl.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://sut.birdmap.top

TS:   await Promise.all(tasks)
来源：http://xto.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lnd.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ysf.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://xhd.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://xne.tianlin.xyz

[O06] 使用进程池
来源：http://gfl.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oyk.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ggm.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://yin.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://xot.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hbs.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cxv.havefunace.top

Ruby: // fork 块
来源：http://egg.yvedp.cn

C#:   Parallel.For
来源：http://ahl.jyoumei.cn

================================================================================
来源：http://bgg.yueranfly.top

P. 常用工具函数
来源：http://mry.zhoulong.xyz

================================================================================
来源：http://tea.jqgfzy.top

[P01] 生成 UUID
来源：http://vuf.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://cfh.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pyv.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://efc.meibo888.top

TS:   crypto.randomUUID()
来源：http://rmg.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://ffw.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://cqp.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://arn.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://rwn.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://wmf.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tgh.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tar.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ucw.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mcr.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://myy.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jqz.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wti.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://boj.yj20258.top

[P03] 生成短随机字符串
来源：http://kwb.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bdd.cheryme.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zye.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ugs.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwh.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qlx.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gaa.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://agq.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cau.nanxuanxn.top

[P04] 求长度
来源：http://asg.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xhq.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pso.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vah.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cte.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://ond.yj20258.top

Go:   len(arr);  len(m)
来源：http://qun.haohaochexian.top

Ruby: x.length;  x.size
来源：http://rkf.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jzn.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://fxb.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vvw.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rbd.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ulr.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sgw.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pdh.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://zfc.ybcxt.top

Ruby: a == b
来源：http://cpe.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ppt.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nwv.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sap.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://lea.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mpp.jqgufenzy.top

TS:   if (x == null) {}
来源：http://ufn.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jyv.hnqzz.top

Go:   if x == nil {}
来源：http://sty.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nmo.zhongyouzk.top

C#:   if (x is null) {}
来源：http://ere.c1oappe.top

[P07] 防抖与节流
来源：http://yay.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ccj.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://iwg.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etm.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hjn.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xst.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://azh.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://afk.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uhc.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://lip.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yjc.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jpc.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sgm.jianghu66.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ats.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nfa.snrcjt.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mbs.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://opa.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ppy.andypj.xyz

================================================================================
来源：http://hky.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nak.meibo888.top

================================================================================
来源：http://vxu.bjfxy.top

[Q01] 创建表
来源：http://djg.zycfv.cn

CREATE TABLE users (
来源：http://emg.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bpo.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://jrc.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://ekx.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zur.zhixingplan.top

);
来源：http://igj.zdbjq.cn

[Q02] 创建带外键的表
来源：http://rdl.zhongyouzk.top

CREATE TABLE orders (
来源：http://ffn.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ngu.bjfxy.top

user_id INT NOT NULL,
来源：http://sse.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://ejm.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wct.xuanzx.com

);
来源：http://jpz.guannengcc.top

[Q03] 增加列
来源：http://sxa.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zyn.haohaochexian.top

[Q04] 修改列类型
来源：http://acz.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sxu.ydjk.org.cn

[Q05] 重命名列
来源：http://ysu.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dfh.wangdashe.top

[Q06] 删除列
来源：http://des.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cfk.jinghuilouyu.cn

[Q07] 删除表
来源：http://tlv.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://nhi.fzhhl.top

[Q08] 创建普通索引
来源：http://gly.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://iam.xuetiantiany.cn

[Q09] 创建唯一索引
来源：http://vlr.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rdu.fzhhl.top

[Q10] 插入单行
来源：http://arg.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jrm.uphjek.com

[Q11] 一次插入多行
来源：http://jwh.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bbx.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://gpr.fzhhl.top

INSERT INTO users (name) VALUES ('C');
来源：http://cfi.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xno.yuanzhike.top

[Q13] 忽略重复插入
来源：http://gmh.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mof.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://tjz.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jdi.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ktx.c1oappe.top

[Q15] 查询全部
来源：http://inq.ppjwa.cn

SELECT * FROM users;
来源：http://auy.yuxming.cn

[Q16] 查询指定列
来源：http://yfg.gaohongyu789.top

SELECT id, name FROM users;
来源：http://afq.guowangkeji.top

[Q17] 条件查询
来源：http://jea.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vkl.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://zoz.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lwd.yonumen.top

[Q19] 范围查询
来源：http://tcf.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cly.epnwcf.com

[Q20] IN 列表
来源：http://plw.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ynx.jinqigfzy.top

[Q21] 空值判断
来源：http://jkf.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yzg.fehbvm.com

[Q22] 排序
来源：http://sqh.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tpy.9152youxi.cn

[Q23] 分页
来源：http://slz.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zoa.mhx1999.top

[Q24] 去重
来源：http://nkp.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://zfv.havefunace.top

[Q25] 只取前 N 条
来源：http://fif.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lcp.hcnkem.com

[Q26] 计数
来源：http://oqj.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://ajc.aibaodan.cn

[Q27] 条件计数
来源：http://txq.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nph.xuanzx.com

[Q28] 求和与平均
来源：http://ztn.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sss.uphjek.com

[Q29] 最大最小值
来源：http://owd.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gxj.zhengqikj.top

[Q30] 分组统计
来源：http://spv.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nnj.bbcook.cn

[Q31] 分组后过滤
来源：http://bbq.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zqt.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://spm.fengsongda.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tlu.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jiv.zhengqikj.top

[Q33] 多列分组
来源：http://hfg.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yql.ydjk.org.cn

[Q34] 每组取第一条
来源：http://ajg.jqgufenzy.top

SELECT * FROM (
来源：http://nnb.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lto.yuxming.cn

) t WHERE rn = 1;
来源：http://ltv.shzxlz.cn

[Q35] 内连接
来源：http://ncb.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ewn.hfpthk.cn

[Q36] 左连接
来源：http://hgw.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uls.zhiwuduotai.top

[Q37] 右连接
来源：http://amc.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sij.jlsjyb.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qwz.xuetiantiany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rga.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://caq.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jye.cashguo.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ovf.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hee.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pwy.jyoumei.cn

[Q41] 多表连接
来源：http://mir.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uad.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://ene.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://jed.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://goj.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://hle.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xwq.vehdjk.com

[Q43] 标量子查询
来源：http://der.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://afg.shzxlz.cn

[Q44] IN 子查询
来源：http://jbj.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cuc.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://rdr.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hbl.shangyingyoupin.top

[Q46] NOT EXISTS 判断不存在
来源：http://zau.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hhp.vehdjk.com

[Q47] 与平均值比较
来源：http://fyy.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dbt.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://kic.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bxa.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://eav.0kj1m.cn

[Q49] 更新单行
来源：http://qjv.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rlh.bbcook.cn

[Q50] 批量更新
来源：http://fbd.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sfm.pycfn.com

[Q51] 用子查询更新
来源：http://qbx.uphjek.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://elq.hongshengwenyu.top

[Q52] 删除指定行
来源：http://wco.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://hzv.nanxuanxn.top

[Q53] 按条件删除
来源：http://zzh.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gso.fengsongda.top

[Q54] 清空表
来源：http://lbo.cucudq.cn

TRUNCATE TABLE logs;
来源：http://jnu.andypj.xyz

[Q55] 排名（并列占位）
来源：http://wbf.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bms.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://lwu.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nto.yuanzhike.top

[Q57] 行号
来源：http://nvy.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://whu.ivvv.top

[Q58] 累计求和
来源：http://dhw.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://chk.gzhubu.top

[Q59] 分组内累计
来源：http://fov.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mqu.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://pgz.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rrb.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qhh.shzxlz.cn

[Q61] 移动平均
来源：http://tfa.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wqd.9152youxi.cn

[Q62] 分组占比
来源：http://xvy.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hxh.cheryme.top

[Q63] 开启事务
来源：http://xxv.guannengcc.top

START TRANSACTION;                -- 或 BEGIN
来源：http://haz.quarkkingdee.top

[Q64] 提交事务
来源：http://uxx.cheryme.top

COMMIT;
来源：http://gla.fengsongda.top

[Q65] 回滚事务
来源：http://mvx.gaohongyu789.top

ROLLBACK;
来源：http://tfe.xuetiantiany.cn

[Q66] 行锁查询
来源：http://acd.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hty.sxryk.cn

[Q67] 设置隔离级别
来源：http://bpu.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sdt.tarul.cn

[Q68] 保存点
来源：http://lgg.hcnkem.com

SAVEPOINT sp1;
来源：http://mev.daria6918.cn

ROLLBACK TO sp1;
来源：http://whq.bbcook.cn

[Q69] 查看执行计划
来源：http://xwo.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wxc.zhongyouzk.top

[Q70] 更新统计信息
来源：http://ueq.daxiang520.top

ANALYZE TABLE users;
来源：http://lfg.nanxinkj.top

[Q71] 查看建表语句
来源：http://gvi.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mej.zhixingplan.top

[Q72] 查看索引
来源：http://zjs.jqgfzy.top

SHOW INDEX FROM users;
来源：http://syb.yongpay.top

[Q73] 查看表状态
来源：http://vdm.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sti.316326.xyz

[Q74] 强制使用索引
来源：http://btg.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vox.jinqigufen.top

[Q75] 日期格式化
来源：http://yff.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oke.fzhhl.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xyr.uphjek.com

[Q76] 按天统计
来源：http://jvu.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lvv.nanxinkj.top

[Q77] 时间加减
来源：http://yet.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mcw.hnqzz.top

[Q78] 当前时间
来源：http://slw.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dxe.nanxuanxn.top

[Q79] 字符串拼接
来源：http://xkn.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ldz.zhongyouzk.top

[Q80] 字符串截取
来源：http://scg.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://edt.yj202588.top

[Q81] 字符串替换
来源：http://ckv.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uex.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://oie.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://upm.wangdashe.top

[Q83] 大小写转换
来源：http://fqb.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://znw.sysykeji.top

[Q84] 去除首尾空格
来源：http://axz.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://kxy.wangshuangyany.cn

[Q85] 数值取整
来源：http://tyd.xylfe.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pqh.yangfankeji.com


<!-- 参考信息 -->