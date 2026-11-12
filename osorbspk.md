代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://oqq.quarkkingdee.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ddi.jinqigfzy.top

JS:   await Promise.all(tasks)
来源：http://fgc.zhaomingkeji.xyz

TS:   await Promise.all(tasks)
来源：http://prc.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ubw.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xfu.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://wnk.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qlz.meibo888.top

[O06] 使用进程池
来源：http://toa.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nby.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fzx.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://awz.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://ify.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ffv.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jem.jinqigfzy.top

Ruby: // fork 块
来源：http://ruc.hnqzz.top

C#:   Parallel.For
来源：http://ddy.shanyushiyangkeji.top

================================================================================
来源：http://kvl.fktsv.cn

P. 常用工具函数
来源：http://kvn.zhijiandao.cn

================================================================================
来源：http://pxl.quarkkingdee.top

[P01] 生成 UUID
来源：http://chy.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://eee.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://itw.c1oappe.top

JS:   crypto.randomUUID()
来源：http://igg.aizwys.cn

TS:   crypto.randomUUID()
来源：http://khx.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://vql.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://rnu.sweek.top

Ruby: SecureRandom.uuid
来源：http://tms.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://zpr.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://okb.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://svf.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://yjd.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hvk.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lww.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qde.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://htn.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ezy.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zhx.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://qjs.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fur.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://klp.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sxo.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ysd.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zqq.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kuo.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://tye.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xmt.xinyue.icu

[P04] 求长度
来源：http://wwq.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pcp.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mij.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nwg.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://izv.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://pgs.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://juz.0kj1m.cn

Ruby: x.length;  x.size
来源：http://dep.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ddc.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://sfa.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ryp.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uyb.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ezd.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://evf.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://njo.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://flq.0kj1m.cn

Ruby: a == b
来源：http://ptc.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gmz.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lgl.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zao.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://qew.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nux.c1oappe.top

TS:   if (x == null) {}
来源：http://loi.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fvr.iojbl.cn

Go:   if x == nil {}
来源：http://hel.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dgn.nanxuanxn.top

C#:   if (x is null) {}
来源：http://ehx.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://dur.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mxb.316326.xyz

PHP:  // 手写时间戳比较
来源：http://oqz.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lpd.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gdb.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://puo.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bzf.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lwb.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mpc.nwbrower.top

[P08] 处理浮点精度问题
来源：http://fve.shanyushiyangtech.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://csi.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lrs.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yxc.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qdr.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://thk.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cro.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://leh.xziqi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qpm.tian-w.cn

================================================================================
来源：http://lev.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ola.jlsjyb.cn

================================================================================
来源：http://ltz.uphjek.com

[Q01] 创建表
来源：http://sfv.gotoacloud.top

CREATE TABLE users (
来源：http://qug.aizwys.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gvd.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://fzx.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://hax.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kiu.316326.xyz

);
来源：http://nii.jyoumei.cn

[Q02] 创建带外键的表
来源：http://anc.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://ejy.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ugn.yongpay.top

user_id INT NOT NULL,
来源：http://lho.smart0.xyz

amount DECIMAL(10, 2),
来源：http://rhh.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vdk.zhiwuduotai.top

);
来源：http://kps.hnxiangtu.top

[Q03] 增加列
来源：http://fgt.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nth.xuanzx.com

[Q04] 修改列类型
来源：http://oee.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pxu.andypj.xyz

[Q05] 重命名列
来源：http://kmg.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ebp.ctjpmb.com

[Q06] 删除列
来源：http://gpu.vehdjk.com

ALTER TABLE users DROP COLUMN age;
来源：http://won.shanyushiyangkeji.top

[Q07] 删除表
来源：http://gdh.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://ymi.meibo888.top

[Q08] 创建普通索引
来源：http://fuh.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rzl.jianghu66.top

[Q09] 创建唯一索引
来源：http://zco.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ssw.bjfxy.top

[Q10] 插入单行
来源：http://nvs.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://scn.316326.xyz

[Q11] 一次插入多行
来源：http://gqh.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://abo.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://nqn.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://syw.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://loc.epnwcf.com

[Q13] 忽略重复插入
来源：http://ljh.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fan.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://jwn.jlsjyb.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hrx.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dth.hysaishi.cn

[Q15] 查询全部
来源：http://yrj.zycfv.cn

SELECT * FROM users;
来源：http://yvg.aibaodan.cn

[Q16] 查询指定列
来源：http://bvc.yueranfly.top

SELECT id, name FROM users;
来源：http://kpl.wangshuangyany.cn

[Q17] 条件查询
来源：http://lwt.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://akf.shzxlz.cn

[Q18] 模糊匹配
来源：http://ilg.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://moi.yj202588.top

[Q19] 范围查询
来源：http://cox.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wlc.yuxming.cn

[Q20] IN 列表
来源：http://yya.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://apq.aizwys.cn

[Q21] 空值判断
来源：http://dro.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://atu.zhongyouzk.top

[Q22] 排序
来源：http://pph.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rhs.gotoacloud.top

[Q23] 分页
来源：http://wpk.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ulr.fehbvm.com

[Q24] 去重
来源：http://biw.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://rxa.hcnkem.com

[Q25] 只取前 N 条
来源：http://vcw.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nng.yj20258888.top

[Q26] 计数
来源：http://zyx.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://ilr.sysykeji.top

[Q27] 条件计数
来源：http://fsy.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hlb.mhx1999.top

[Q28] 求和与平均
来源：http://gen.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://htp.feifeiyinyue.top

[Q29] 最大最小值
来源：http://jui.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yby.daria6918.cn

[Q30] 分组统计
来源：http://irw.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ukl.daxiang520.top

[Q31] 分组后过滤
来源：http://ctq.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ssm.quarkkingdee.top

[Q32] 分组拼接字符串
来源：http://jjo.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jhp.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jzu.hfpthk.cn

[Q33] 多列分组
来源：http://lxt.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tuu.zhongyouzk.top

[Q34] 每组取第一条
来源：http://iro.jqgfzy.top

SELECT * FROM (
来源：http://oid.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nhe.jqgfzy.top

) t WHERE rn = 1;
来源：http://cfn.chenzaomai.com

[Q35] 内连接
来源：http://bhb.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tcv.yvedp.cn

[Q36] 左连接
来源：http://wmd.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vuq.hcnkem.com

[Q37] 右连接
来源：http://vat.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cck.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://irr.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://chl.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://imo.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eel.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://spo.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pap.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uqi.ehwqpu.com

[Q41] 多表连接
来源：http://xgv.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ovy.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://qjl.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://cum.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://rfq.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://alu.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kvv.yangfankeji.com

[Q43] 标量子查询
来源：http://mxt.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uwu.vehdjk.com

[Q44] IN 子查询
来源：http://byx.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nkr.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://gxq.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vyv.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://zpe.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aoc.yvedp.cn

[Q47] 与平均值比较
来源：http://vfw.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://trv.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://ytx.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wsi.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://jjt.jqgufenzy.top

[Q49] 更新单行
来源：http://jfq.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://slj.zhixingplan.top

[Q50] 批量更新
来源：http://qoj.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pda.ybcxt.top

[Q51] 用子查询更新
来源：http://xsi.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qzi.yonumen.top

[Q52] 删除指定行
来源：http://ipg.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://rmf.ivvv.top

[Q53] 按条件删除
来源：http://ozw.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nac.zhijiandao.cn

[Q54] 清空表
来源：http://efy.gaohongyu789.top

TRUNCATE TABLE logs;
来源：http://viq.yfazqb.com

[Q55] 排名（并列占位）
来源：http://cdi.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pjb.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://owg.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bgj.jlsjyb.cn

[Q57] 行号
来源：http://wvv.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hjp.dashuyun.cn

[Q58] 累计求和
来源：http://hqn.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xas.ydzc1.top

[Q59] 分组内累计
来源：http://kld.gotoacloud.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sjr.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://hnv.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zpn.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gwh.ivvv.top

[Q61] 移动平均
来源：http://jve.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dtn.316326.xyz

[Q62] 分组占比
来源：http://pai.daria6918.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ihn.chenlongwang.top

[Q63] 开启事务
来源：http://cjb.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://csk.yj20258888.top

[Q64] 提交事务
来源：http://igq.xuetiantiany.cn

COMMIT;
来源：http://acn.wangdashe.top

[Q65] 回滚事务
来源：http://owi.zhaomingkeji.xyz

ROLLBACK;
来源：http://sch.dianchejie.cn

[Q66] 行锁查询
来源：http://ihr.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oah.c1oappe.top

[Q67] 设置隔离级别
来源：http://xcn.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cbb.shangyingyoupin.top

[Q68] 保存点
来源：http://seq.birdmap.top

SAVEPOINT sp1;
来源：http://kfb.c1oappe.top

ROLLBACK TO sp1;
来源：http://jlz.xuanzx.com

[Q69] 查看执行计划
来源：http://qtd.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sqg.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://tac.hfpthk.cn

ANALYZE TABLE users;
来源：http://itr.tian-w.cn

[Q71] 查看建表语句
来源：http://mtd.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bks.pycfn.com

[Q72] 查看索引
来源：http://jhw.hammf.cn

SHOW INDEX FROM users;
来源：http://evx.bjfxy.top

[Q73] 查看表状态
来源：http://umk.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nmz.cashguo.top

[Q74] 强制使用索引
来源：http://jyg.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qqu.jinqigfzy.top

[Q75] 日期格式化
来源：http://vcl.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://okp.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ggw.birdmap.top

[Q76] 按天统计
来源：http://ipp.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://clj.kuanghao11.cn

[Q77] 时间加减
来源：http://ssv.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ayz.hcnkem.com

[Q78] 当前时间
来源：http://uro.shzxlz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kly.meibo888.top

[Q79] 字符串拼接
来源：http://fgb.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xpa.yanxiufei.cn

[Q80] 字符串截取
来源：http://zyw.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vmo.sjlbkw.cn

[Q81] 字符串替换
来源：http://wwn.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://isv.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://vsk.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://irr.xylfe.cn

[Q83] 大小写转换
来源：http://dmn.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iob.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://mja.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://ykh.hfpthk.cn

[Q85] 数值取整
来源：http://puy.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bpd.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://utu.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ctc.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://tia.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yym.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://akl.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wxt.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kvf.sxryk.cn

[Q89] 判断表是否存在
来源：http://cif.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rxu.cucudq.cn

[Q90] 生成序号列
来源：http://ebu.mhx1999.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://czt.yanxiufei.cn

================================================================================
来源：http://xpr.cashguo.top


<!-- 参考信息 -->