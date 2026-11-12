代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://uab.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://baw.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://iby.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://yxf.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qxw.tarul.cn

JS:   async function f() { await g(); }
来源：http://mzn.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rwm.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lsx.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://syn.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oie.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://lxg.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://cdg.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://njs.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jll.cheryme.top

JS:   await Promise.all(tasks)
来源：http://yvy.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://ifi.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vae.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oct.yongpay.top

Ruby: threads.map(&:join)
来源：http://eum.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yls.iojbl.cn

[O06] 使用进程池
来源：http://tie.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tlr.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://orb.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://ctd.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://qnd.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fwe.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ykh.jianghu66.top

Ruby: // fork 块
来源：http://slw.zycfv.cn

C#:   Parallel.For
来源：http://swt.xziqi.cn

================================================================================
来源：http://rnt.chenjidiqi.icu

P. 常用工具函数
来源：http://owx.ehwqpu.com

================================================================================
来源：http://vfy.yj202588.top

[P01] 生成 UUID
来源：http://ypd.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://tby.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tqq.gaohongyu789.top

JS:   crypto.randomUUID()
来源：http://qpk.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://ckv.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://hay.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://ihm.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://fdm.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://lnd.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://wdj.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cnv.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dcd.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tap.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dsu.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://moz.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kwr.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ddr.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://imm.zycfv.cn

[P03] 生成短随机字符串
来源：http://zvs.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bpg.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yrg.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xox.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bjp.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wdx.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aio.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gzz.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mux.zhaomingkeji.xyz

[P04] 求长度
来源：http://cse.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pjw.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oyb.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://isn.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahi.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://gya.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://ecf.jqgfzy.top

Ruby: x.length;  x.size
来源：http://tbk.zdbjq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qau.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://kqr.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zac.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wxl.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wmy.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ggy.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vdf.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://vcy.yvedp.cn

Ruby: a == b
来源：http://ylh.yonumen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dym.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xcx.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rom.yongpay.top

PHP:  if (empty($x)) {}
来源：http://flm.jinqigufen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lcu.jyoumei.cn

TS:   if (x == null) {}
来源：http://whj.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tba.epnwcf.com

Go:   if x == nil {}
来源：http://ngz.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gzm.zhongyouzk.top

C#:   if (x is null) {}
来源：http://nnf.jinyuanbaomall.cn

[P07] 防抖与节流
来源：http://upm.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jxe.xylfe.cn

PHP:  // 手写时间戳比较
来源：http://jap.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bpt.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcb.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cvb.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wvj.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xvt.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zzz.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://wyl.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bmj.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dhi.jinqigfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lqc.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ieu.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://deg.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kyl.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dtq.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vhn.ivvv.top

================================================================================
来源：http://wwo.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gyc.hywenlv.cn

================================================================================
来源：http://wzc.xinyue.icu

[Q01] 创建表
来源：http://uuv.yuxming.cn

CREATE TABLE users (
来源：http://llz.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cyx.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://dzt.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://rzr.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iss.jinqigfzy.top

);
来源：http://sje.mhx1999.top

[Q02] 创建带外键的表
来源：http://ifi.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://kdg.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dxb.yangfankeji.com

user_id INT NOT NULL,
来源：http://fgt.andypj.xyz

amount DECIMAL(10, 2),
来源：http://kyi.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://prm.iojbl.cn

);
来源：http://ujk.quarkkingdee.top

[Q03] 增加列
来源：http://woj.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dfx.birdmap.top

[Q04] 修改列类型
来源：http://ryb.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kur.316326.xyz

[Q05] 重命名列
来源：http://hoz.vehdjk.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yru.yonumen.top

[Q06] 删除列
来源：http://vfs.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qsr.yj20258.top

[Q07] 删除表
来源：http://bvd.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://ivk.9152youxi.cn

[Q08] 创建普通索引
来源：http://heu.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zyl.c1oappe.top

[Q09] 创建唯一索引
来源：http://rbc.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vrd.chenjidiqi.icu

[Q10] 插入单行
来源：http://vmj.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oyp.vehdjk.com

[Q11] 一次插入多行
来源：http://uvd.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cef.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://rki.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zsp.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qwz.bbcook.cn

[Q13] 忽略重复插入
来源：http://poz.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hyu.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://mrj.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tnv.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jal.jinqigfzy.top

[Q15] 查询全部
来源：http://gpg.sweek.top

SELECT * FROM users;
来源：http://tbt.nanxinkj.top

[Q16] 查询指定列
来源：http://jiz.svipenyu.cn

SELECT id, name FROM users;
来源：http://mti.jinqigufen.top

[Q17] 条件查询
来源：http://ajr.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://duz.fehbvm.com

[Q18] 模糊匹配
来源：http://yjb.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://viu.mhx1999.top

[Q19] 范围查询
来源：http://qdf.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://moe.sysykeji.top

[Q20] IN 列表
来源：http://tep.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ehb.shangyingyoupin.top

[Q21] 空值判断
来源：http://kzf.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://idj.gogol.net.cn

[Q22] 排序
来源：http://gtk.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uza.epnwcf.com

[Q23] 分页
来源：http://ofl.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iww.gogol.net.cn

[Q24] 去重
来源：http://wkl.fanxiaobao.xyz

SELECT DISTINCT city FROM users;
来源：http://ajx.jqgfzy.top

[Q25] 只取前 N 条
来源：http://hbv.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fvd.52xcode.cn

[Q26] 计数
来源：http://kop.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://rpw.cqqwz.cn

[Q27] 条件计数
来源：http://lhj.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fgf.epnwcf.com

[Q28] 求和与平均
来源：http://efs.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rrn.cheryme.top

[Q29] 最大最小值
来源：http://axp.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cce.iojbl.cn

[Q30] 分组统计
来源：http://gmg.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xxg.xuanzx.com

[Q31] 分组后过滤
来源：http://zre.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ens.daria6918.cn

[Q32] 分组拼接字符串
来源：http://vfh.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fiz.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bhq.cqqwz.cn

[Q33] 多列分组
来源：http://wcx.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uya.fengsongda.top

[Q34] 每组取第一条
来源：http://ojy.hysaishi.cn

SELECT * FROM (
来源：http://kxn.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://has.316326.xyz

) t WHERE rn = 1;
来源：http://tsm.kuanghao11.cn

[Q35] 内连接
来源：http://fpy.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kod.zhengqikj.top

[Q36] 左连接
来源：http://arx.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ftv.ybcxt.top

[Q37] 右连接
来源：http://but.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uqh.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cql.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://spy.shuidangran.top

[Q39] 自连接（查上下级）
来源：http://cvj.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://flj.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bkw.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vlt.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nxq.birdmap.top

[Q41] 多表连接
来源：http://wtg.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dax.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://apo.xuanzx.com

JOIN products p ON p.id = o.product_id;
来源：http://ncs.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://pnx.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://zlf.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xmx.xuetiantiany.cn

[Q43] 标量子查询
来源：http://ujo.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kqo.ydjk.org.cn

[Q44] IN 子查询
来源：http://qsw.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ova.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://igf.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jiz.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://mus.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uuc.ydzc1.top

[Q47] 与平均值比较
来源：http://vtv.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rbp.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://aks.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bla.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://gej.daria6918.cn

[Q49] 更新单行
来源：http://cvx.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rwu.yuxming.cn

[Q50] 批量更新
来源：http://elf.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vip.52xcode.cn

[Q51] 用子查询更新
来源：http://iwd.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://urs.xziqi.cn

[Q52] 删除指定行
来源：http://pds.epnwcf.com

DELETE FROM users WHERE id = 10;
来源：http://qvx.jlsjyb.cn

[Q53] 按条件删除
来源：http://lao.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kpk.yvedp.cn

[Q54] 清空表
来源：http://nfe.xinyue.icu

TRUNCATE TABLE logs;
来源：http://gyb.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://vhi.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://moy.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://vxh.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://krz.dianchejie.cn

[Q57] 行号
来源：http://kiv.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mro.jinghuilouyu.cn

[Q58] 累计求和
来源：http://smx.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://guj.yj202588.top

[Q59] 分组内累计
来源：http://rqp.pengpengdd.cyou

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://myc.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://sgn.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://efq.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rzb.xuanzx.com

[Q61] 移动平均
来源：http://lec.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yap.quarkkingdee.top

[Q62] 分组占比
来源：http://vzw.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dqw.chenlongwang.top

[Q63] 开启事务
来源：http://cbp.jinyuanbaomall.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lii.yonumen.top

[Q64] 提交事务
来源：http://wni.gzhubu.top

COMMIT;
来源：http://qba.kuanghao11.cn

[Q65] 回滚事务
来源：http://zts.ivvv.top

ROLLBACK;
来源：http://hto.yvedp.cn

[Q66] 行锁查询
来源：http://byg.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wwr.yongpay.top

[Q67] 设置隔离级别
来源：http://eej.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wna.xuetiantiany.cn

[Q68] 保存点
来源：http://kel.chenzaomai.com

SAVEPOINT sp1;
来源：http://mqf.ppjwa.cn

ROLLBACK TO sp1;
来源：http://ege.epnwcf.com

[Q69] 查看执行计划
来源：http://gme.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yyf.shuidangran.top

[Q70] 更新统计信息
来源：http://mbk.zhixingplan.top

ANALYZE TABLE users;
来源：http://zgr.redwolf501.top

[Q71] 查看建表语句
来源：http://xzc.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ord.jyoumei.cn

[Q72] 查看索引
来源：http://xfs.hcnkem.com

SHOW INDEX FROM users;
来源：http://fgm.tian-w.cn

[Q73] 查看表状态
来源：http://jhb.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dul.9152youxi.cn

[Q74] 强制使用索引
来源：http://mmf.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cch.nwbrower.top

[Q75] 日期格式化
来源：http://jci.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://krv.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lbi.cucudq.cn

[Q76] 按天统计
来源：http://puc.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zsh.yongpay.top

[Q77] 时间加减
来源：http://jxa.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qam.xinyue.icu

[Q78] 当前时间
来源：http://uoj.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rwb.ydjk.org.cn

[Q79] 字符串拼接
来源：http://tfu.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jnf.bbcook.cn

[Q80] 字符串截取
来源：http://dru.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rbv.cashguo.top

[Q81] 字符串替换
来源：http://zer.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tef.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://clt.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://daw.aizwys.cn

[Q83] 大小写转换
来源：http://okw.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rgf.daxiang520.top

[Q84] 去除首尾空格
来源：http://lao.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://nvm.dianchejie.cn

[Q85] 数值取整
来源：http://zhc.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pxb.jinqigfzy.top


<!-- 参考信息 -->