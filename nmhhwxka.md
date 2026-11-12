代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rxn.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://uyz.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://viz.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://adq.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://nwk.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ypk.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://kay.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://rgc.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://siy.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yxy.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://nbn.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://idq.andypj.xyz

[O06] 使用进程池
来源：http://pvg.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ayw.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xzp.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://aot.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://onn.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lph.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hmu.xuetiantiany.cn

Ruby: // fork 块
来源：http://auf.yongpay.top

C#:   Parallel.For
来源：http://iss.hongshengwenyu.top

================================================================================
来源：http://tqh.316326.xyz

P. 常用工具函数
来源：http://zyl.fengsongda.top

================================================================================
来源：http://psj.hywenlv.cn

[P01] 生成 UUID
来源：http://wun.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://tts.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nqo.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://dxp.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://trq.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://hld.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://djo.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://xrg.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://wrs.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://ivi.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jue.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://qcd.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ubi.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://quc.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://thj.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tqr.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kxm.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bbx.nwbrower.top

[P03] 生成短随机字符串
来源：http://zwv.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lmj.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rsk.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://amj.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ipm.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nsk.gaohongyu789.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rbk.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://cni.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rkh.yanxiufei.cn

[P04] 求长度
来源：http://puw.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vbz.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wri.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tsj.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ipx.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://gcg.aizwys.cn

Go:   len(arr);  len(m)
来源：http://hpf.ivvv.top

Ruby: x.length;  x.size
来源：http://vzr.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dyx.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://fgu.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://puj.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ufs.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uki.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nwm.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://utd.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://two.jyoumei.cn

Ruby: a == b
来源：http://iew.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ass.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pbm.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://byk.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://aon.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cnd.ctjpmb.com

TS:   if (x == null) {}
来源：http://vcx.birdmap.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ayw.redwolf501.top

Go:   if x == nil {}
来源：http://wbg.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kcv.shuidangran.top

C#:   if (x is null) {}
来源：http://hnr.dianchejie.cn

[P07] 防抖与节流
来源：http://vzu.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bhd.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://zzf.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkm.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ygj.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qnf.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://enk.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://stg.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://avy.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://aua.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ndu.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dmk.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qgx.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vrs.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://shr.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://itj.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tzv.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ess.52xcode.cn

================================================================================
来源：http://bag.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wtm.zhijiandao.cn

================================================================================
来源：http://bsw.hongshengwenyu.top

[Q01] 创建表
来源：http://pfx.sxryk.cn

CREATE TABLE users (
来源：http://zpj.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xav.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://ggi.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://nhs.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://euv.wangshuangyany.cn

);
来源：http://eas.smart0.xyz

[Q02] 创建带外键的表
来源：http://ghg.pengpengdd.cyou

CREATE TABLE orders (
来源：http://ezg.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dfu.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://nbi.xinyue.icu

amount DECIMAL(10, 2),
来源：http://rye.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rht.nanxinkj.top

);
来源：http://phk.yueranfly.top

[Q03] 增加列
来源：http://uvg.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tpq.chenlongwang.top

[Q04] 修改列类型
来源：http://kjd.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sag.zhixingplan.top

[Q05] 重命名列
来源：http://kqj.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gmr.yvedp.cn

[Q06] 删除列
来源：http://xan.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://ltk.xziqi.cn

[Q07] 删除表
来源：http://zfu.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://oll.haohaochexian.top

[Q08] 创建普通索引
来源：http://qcy.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://stw.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://klg.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pbo.fengsongda.top

[Q10] 插入单行
来源：http://fzn.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://czs.zhongyouzk.top

[Q11] 一次插入多行
来源：http://fzq.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://llz.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://vdh.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://vkh.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fmu.hfpthk.cn

[Q13] 忽略重复插入
来源：http://oor.vqdsnc.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xdl.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://ern.iojbl.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://asb.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pdl.zycfv.cn

[Q15] 查询全部
来源：http://qhp.yonumen.top

SELECT * FROM users;
来源：http://ivv.yonumen.top

[Q16] 查询指定列
来源：http://try.yvedp.cn

SELECT id, name FROM users;
来源：http://yqq.iojbl.cn

[Q17] 条件查询
来源：http://trv.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dgm.nanxuanxn.top

[Q18] 模糊匹配
来源：http://jpq.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oss.yuxming.cn

[Q19] 范围查询
来源：http://sdn.uphjek.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iel.ehwqpu.com

[Q20] IN 列表
来源：http://itz.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eft.xylfe.cn

[Q21] 空值判断
来源：http://iay.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gpm.svipenyu.cn

[Q22] 排序
来源：http://gec.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vdc.hesvh.cn

[Q23] 分页
来源：http://xsv.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yih.fzhhl.top

[Q24] 去重
来源：http://njo.hammf.cn

SELECT DISTINCT city FROM users;
来源：http://mrw.hammf.cn

[Q25] 只取前 N 条
来源：http://rnl.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://evo.hesvh.cn

[Q26] 计数
来源：http://cdr.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://tpt.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://ukv.bbcook.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hrs.snrcjt.cn

[Q28] 求和与平均
来源：http://cvs.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cpx.mhx1999.top

[Q29] 最大最小值
来源：http://spo.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://gag.yangfankeji.com

[Q30] 分组统计
来源：http://nvo.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://amn.xziqi.cn

[Q31] 分组后过滤
来源：http://xtc.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lva.hnqzz.top

[Q32] 分组拼接字符串
来源：http://wdp.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://csi.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://spw.zhengqikj.top

[Q33] 多列分组
来源：http://zil.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oip.sjlbkw.cn

[Q34] 每组取第一条
来源：http://oax.yj202588.top

SELECT * FROM (
来源：http://reg.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bww.hesvh.cn

) t WHERE rn = 1;
来源：http://pql.yueranfly.top

[Q35] 内连接
来源：http://ncc.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qnn.meibo888.top

[Q36] 左连接
来源：http://amn.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://neg.zdbjq.cn

[Q37] 右连接
来源：http://uij.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ccr.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://onl.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hhg.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://khz.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://oom.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vsy.jinghuilouyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tlc.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bwb.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://hcc.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://sgm.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://vrf.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://ugb.yonumen.top

[Q42] 连接条件附加过滤
来源：http://lte.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://dbt.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uku.cashguo.top

[Q43] 标量子查询
来源：http://och.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sfp.pengpengdd.cyou

[Q44] IN 子查询
来源：http://gea.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bdi.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://ixn.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hrc.zhongyouzk.top

[Q46] NOT EXISTS 判断不存在
来源：http://hrh.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lih.yongpay.top

[Q47] 与平均值比较
来源：http://cmj.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qni.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://uof.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://frs.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://izq.haohaochexian.top

[Q49] 更新单行
来源：http://uxr.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zli.yueranfly.top

[Q50] 批量更新
来源：http://qsx.yj20258888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wbv.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://fuz.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tvx.hammf.cn

[Q52] 删除指定行
来源：http://knt.daxiang520.top

DELETE FROM users WHERE id = 10;
来源：http://dlv.zhongyouzk.top

[Q53] 按条件删除
来源：http://pjk.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://boz.guowangkeji.top

[Q54] 清空表
来源：http://jfh.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://gii.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://apv.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hii.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://dfb.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ssc.9152youxi.cn

[Q57] 行号
来源：http://puz.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rti.gzhubu.top

[Q58] 累计求和
来源：http://izg.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bpf.cashguo.top

[Q59] 分组内累计
来源：http://wcl.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rsx.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://luk.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qwe.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xsu.yfazqb.com

[Q61] 移动平均
来源：http://mmi.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lzk.yj20258888.top

[Q62] 分组占比
来源：http://faw.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eyn.pengpengdd.cyou

[Q63] 开启事务
来源：http://nsr.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ycl.zhengqikj.top

[Q64] 提交事务
来源：http://omk.sjlbkw.cn

COMMIT;
来源：http://gpx.xziqi.cn

[Q65] 回滚事务
来源：http://hhh.redwolf501.top

ROLLBACK;
来源：http://pml.mhx1999.top

[Q66] 行锁查询
来源：http://dys.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mml.jiagoushi.top

[Q67] 设置隔离级别
来源：http://xgs.feifeiyinyue.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eip.hcnkem.com

[Q68] 保存点
来源：http://bwy.yj20258888.top

SAVEPOINT sp1;
来源：http://jfy.cashguo.top

ROLLBACK TO sp1;
来源：http://zjx.sysykeji.top

[Q69] 查看执行计划
来源：http://kdy.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ujw.yangfankeji.com

[Q70] 更新统计信息
来源：http://btx.yfazqb.com

ANALYZE TABLE users;
来源：http://ojt.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://juz.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cbl.hnqzz.top

[Q72] 查看索引
来源：http://oms.chenlongwang.top

SHOW INDEX FROM users;
来源：http://hsq.uphjek.com

[Q73] 查看表状态
来源：http://ian.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kdf.cashguo.top

[Q74] 强制使用索引
来源：http://dcm.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://waf.cheryme.top

[Q75] 日期格式化
来源：http://vel.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bdy.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://avp.daxiang520.top

[Q76] 按天统计
来源：http://zmk.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hti.redwolf501.top

[Q77] 时间加减
来源：http://fbj.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ldk.fktsv.cn

[Q78] 当前时间
来源：http://toz.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mya.fktsv.cn

[Q79] 字符串拼接
来源：http://sek.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://scr.yueranfly.top

[Q80] 字符串截取
来源：http://zum.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jyr.chenzaomai.com

[Q81] 字符串替换
来源：http://ump.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://har.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://ict.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fyk.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://gya.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lms.bjfxy.top

[Q84] 去除首尾空格
来源：http://bgf.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://gis.uphjek.com

[Q85] 数值取整
来源：http://lcg.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dqn.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://vqs.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hcj.pycfn.com

[Q87] JSON 字段做条件
来源：http://byo.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xkw.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://gfa.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hiu.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bxi.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://ybt.tanke756.top


<!-- 参考信息 -->