代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://ajb.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gzt.xuetiantiany.cn

JS:   await Promise.all(tasks)
来源：http://mng.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://qvv.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hoc.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://job.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://ztx.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://cpx.fzhhl.top

[O06] 使用进程池
来源：http://sdh.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kal.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rsk.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://fjn.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://ufy.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yvt.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mag.xylfe.cn

Ruby: // fork 块
来源：http://wgl.havefunace.top

C#:   Parallel.For
来源：http://oxt.zycfv.cn

================================================================================
来源：http://hog.pycfn.com

P. 常用工具函数
来源：http://cdt.yuanzhike.top

================================================================================
来源：http://mqa.aizwys.cn

[P01] 生成 UUID
来源：http://rwu.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://ptd.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cng.pycfn.com

JS:   crypto.randomUUID()
来源：http://fti.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://vct.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://syn.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://rja.tanke756.top

Ruby: SecureRandom.uuid
来源：http://wxd.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://asz.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://krb.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yna.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://orm.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nmd.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dhk.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wgs.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://smg.guannengcc.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oza.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yjt.xuanzx.com

[P03] 生成短随机字符串
来源：http://bdk.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lcr.xuetiantiany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gaa.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tyi.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wcm.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xnp.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kyn.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cjc.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ock.ivvv.top

[P04] 求长度
来源：http://bcs.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dju.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lbb.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uqf.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qqr.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://tkm.hnqzz.top

Go:   len(arr);  len(m)
来源：http://sdr.birdmap.top

Ruby: x.length;  x.size
来源：http://dse.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zcw.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://yee.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://efk.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tmh.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bsy.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qee.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xcz.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://kwj.0kj1m.cn

Ruby: a == b
来源：http://hyd.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qwp.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qfa.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jpb.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://hwe.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tdw.yj202588.top

TS:   if (x == null) {}
来源：http://wkr.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kjj.guannengcc.top

Go:   if x == nil {}
来源：http://bgx.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yqz.yonumen.top

C#:   if (x is null) {}
来源：http://xyi.316326.xyz

[P07] 防抖与节流
来源：http://zsx.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sfu.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://giy.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://beg.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dkc.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rja.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wco.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cvc.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hkg.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://gkm.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://job.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hox.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vkg.nanxuanxn.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hvw.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sep.sufxvd.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://grv.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://voj.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gns.zhengqikj.top

================================================================================
来源：http://kgh.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vdg.jinyuanbaomall.cn

================================================================================
来源：http://xrp.ehwqpu.com

[Q01] 创建表
来源：http://dtg.dianchejie.cn

CREATE TABLE users (
来源：http://qdv.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nek.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://nbt.daria6918.cn

email VARCHAR(100) UNIQUE,
来源：http://yft.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fxk.nanxuanxn.top

);
来源：http://qqe.daria6918.cn

[Q02] 创建带外键的表
来源：http://tfa.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://lol.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://moq.ydjk.org.cn

user_id INT NOT NULL,
来源：http://ymf.jyoumei.cn

amount DECIMAL(10, 2),
来源：http://wqu.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://duz.zhengqikj.top

);
来源：http://wja.daria6918.cn

[Q03] 增加列
来源：http://pgk.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jty.ydjk.org.cn

[Q04] 修改列类型
来源：http://hng.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tfs.aizwys.cn

[Q05] 重命名列
来源：http://zol.c1oappe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ltj.fzhhl.top

[Q06] 删除列
来源：http://xfg.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://kkd.hnxiangtu.top

[Q07] 删除表
来源：http://btu.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://ahd.yueranfly.top

[Q08] 创建普通索引
来源：http://skm.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yju.chenlongwang.top

[Q09] 创建唯一索引
来源：http://vea.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mfb.meibo888.top

[Q10] 插入单行
来源：http://vhh.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mjl.hesvh.cn

[Q11] 一次插入多行
来源：http://vfa.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gjh.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://lgk.chenjidiqi.icu

INSERT INTO users (name) VALUES ('C');
来源：http://ixe.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jhw.ehwqpu.com

[Q13] 忽略重复插入
来源：http://zym.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fam.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://cwf.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nod.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zge.zhoulong.xyz

[Q15] 查询全部
来源：http://vsy.ybcxt.top

SELECT * FROM users;
来源：http://kiy.hesvh.cn

[Q16] 查询指定列
来源：http://gmw.epnwcf.com

SELECT id, name FROM users;
来源：http://jcb.pengpengdd.cyou

[Q17] 条件查询
来源：http://bbo.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jdd.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://jjj.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ksc.sysykeji.top

[Q19] 范围查询
来源：http://zsv.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sjk.vqdsnc.cn

[Q20] IN 列表
来源：http://emq.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vqg.yj20258888.top

[Q21] 空值判断
来源：http://iai.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://orr.ybcxt.top

[Q22] 排序
来源：http://wig.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tyn.jinyuanbaomall.cn

[Q23] 分页
来源：http://ssm.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hwp.zhoulong.xyz

[Q24] 去重
来源：http://lak.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://zdd.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://kpx.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://luh.ywan-chungtsiang.top

[Q26] 计数
来源：http://bdt.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://wfd.fanxiaobao.xyz

[Q27] 条件计数
来源：http://ljm.xziqi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jsp.yfazqb.com

[Q28] 求和与平均
来源：http://fif.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pnb.gaohongyu789.top

[Q29] 最大最小值
来源：http://tzi.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lsv.hysaishi.cn

[Q30] 分组统计
来源：http://yua.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lxj.chenzaomai.com

[Q31] 分组后过滤
来源：http://lot.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jja.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://fnh.ywan-chungtsiang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ept.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://osa.birdmap.top

[Q33] 多列分组
来源：http://czu.xziqi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vva.ehwqpu.com

[Q34] 每组取第一条
来源：http://vqm.zhengqikj.top

SELECT * FROM (
来源：http://lye.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fsi.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://byh.yueranfly.top

[Q35] 内连接
来源：http://lqa.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nlk.pengpengdd.cyou

[Q36] 左连接
来源：http://zuw.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tch.fengsongda.top

[Q37] 右连接
来源：http://hxx.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mqu.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zhj.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pxc.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://aim.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://agu.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oxs.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pmx.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ryt.hfpthk.cn

[Q41] 多表连接
来源：http://zvw.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://eby.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://whi.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://jyg.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://rdz.kuanghao11.cn

SELECT u.name, o.amount FROM users u
来源：http://tib.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hrk.iojbl.cn

[Q43] 标量子查询
来源：http://fyv.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ntl.tianlin.xyz

[Q44] IN 子查询
来源：http://rxe.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zpy.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://xhu.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rvg.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cqb.cqqwz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bvj.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://dzo.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wsc.quarkkingdee.top

[Q48] CTE 公用表表达式
来源：http://bdh.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mbj.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://big.ydzc1.top

[Q49] 更新单行
来源：http://udu.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wdd.zdqjudy.top

[Q50] 批量更新
来源：http://rmr.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sib.yangfankeji.com

[Q51] 用子查询更新
来源：http://wwk.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ooi.pengpengdd.cyou

[Q52] 删除指定行
来源：http://hqh.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://gjw.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://crt.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gid.ctjpmb.com

[Q54] 清空表
来源：http://sol.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://qpb.daxiang520.top

[Q55] 排名（并列占位）
来源：http://fqp.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://utz.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://jno.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lsu.yj20258888.top

[Q57] 行号
来源：http://wrx.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rdv.aizwys.cn

[Q58] 累计求和
来源：http://dhh.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nrw.jqgfzy.top

[Q59] 分组内累计
来源：http://wui.gotoacloud.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://koy.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://dwl.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zjw.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oal.hammf.cn

[Q61] 移动平均
来源：http://onx.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pjj.chenzaomai.com

[Q62] 分组占比
来源：http://hcd.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://esk.sweek.top

[Q63] 开启事务
来源：http://tiz.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ckf.nanxinkj.top

[Q64] 提交事务
来源：http://luo.zhijiandao.cn

COMMIT;
来源：http://ura.fktsv.cn

[Q65] 回滚事务
来源：http://iye.hongshengwenyu.top

ROLLBACK;
来源：http://anz.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://vhy.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mzm.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://cvr.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pue.yonumen.top

[Q68] 保存点
来源：http://enx.yuxming.cn

SAVEPOINT sp1;
来源：http://qae.zhixingplan.top

ROLLBACK TO sp1;
来源：http://odz.zhoulong.xyz

[Q69] 查看执行计划
来源：http://ivk.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gbz.guannengcc.top

[Q70] 更新统计信息
来源：http://ovb.mhx1999.top

ANALYZE TABLE users;
来源：http://xhd.yanxiufei.cn

[Q71] 查看建表语句
来源：http://yxn.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://msa.sjlbkw.cn

[Q72] 查看索引
来源：http://dzl.jqgfzy.top

SHOW INDEX FROM users;
来源：http://wia.hesvh.cn

[Q73] 查看表状态
来源：http://lmx.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zmo.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://jcu.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wyo.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://jhn.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eyx.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jub.cheryme.top

[Q76] 按天统计
来源：http://fpk.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jze.smart0.xyz

[Q77] 时间加减
来源：http://elv.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xbn.tianlin.xyz

[Q78] 当前时间
来源：http://zlr.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zhi.hywenlv.cn

[Q79] 字符串拼接
来源：http://nrt.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qfg.316326.xyz

[Q80] 字符串截取
来源：http://rfg.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uru.fzhhl.top

[Q81] 字符串替换
来源：http://pqi.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dur.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://lqk.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fwh.tarul.cn

[Q83] 大小写转换
来源：http://jbn.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eus.shzxlz.cn

[Q84] 去除首尾空格
来源：http://nyj.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://dpj.tarul.cn

[Q85] 数值取整
来源：http://hre.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pkb.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://mtw.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://adu.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://cth.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bmo.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://qop.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gyy.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tnj.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://kcv.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gpb.guowangkeji.top

[Q90] 生成序号列
来源：http://lll.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://skh.bjfxy.top

================================================================================
来源：http://yez.cqqwz.cn


<!-- 参考信息 -->