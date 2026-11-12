代发 wailian999

[O02] 使用线程池
来源：http://vzw.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ixt.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xff.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://dci.daxiang520.top

TS:   // worker_threads 线程池
来源：http://hxv.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://flh.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gvw.ctjpmb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iah.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bdt.zycfv.cn

[O03] 加锁保护共享数据
来源：http://ffe.wangdashe.top

Py:   with lock: shared += 1
来源：http://hzh.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://qyg.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://may.yuxming.cn

TS:   // 同 JS
来源：http://dlg.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://ddz.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hkr.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ghz.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://pdg.vehdjk.com

[O04] 定义异步函数并等待
来源：http://fij.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://eol.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cdq.mhx1999.top

JS:   async function f() { await g(); }
来源：http://lfc.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ygp.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fsh.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wja.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://gja.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://wsz.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://imx.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://qnw.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tnv.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://fnc.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://swg.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zwc.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zjh.bjfxy.top

Ruby: threads.map(&:join)
来源：http://ecg.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qcq.dashuyun.cn

[O06] 使用进程池
来源：http://kkt.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rua.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://eua.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://wil.0kj1m.cn

TS:   // child_process / cluster 模块
来源：http://njg.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qdd.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gpv.jiagoushi.top

Ruby: // fork 块
来源：http://iit.jinqigufen.top

C#:   Parallel.For
来源：http://les.0kj1m.cn

================================================================================
来源：http://trk.cheryme.top

P. 常用工具函数
来源：http://txf.dianchejie.cn

================================================================================
来源：http://rwe.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://riw.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://afx.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://icp.tarul.cn

JS:   crypto.randomUUID()
来源：http://elm.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://ccl.xziqi.cn

Java: UUID.randomUUID().toString()
来源：http://gzp.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://gef.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://uvp.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://frk.zhaomingkeji.xyz

[P02] MD5 / SHA256 摘要
来源：http://chf.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ryo.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vfp.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gtl.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://emg.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vrm.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mnz.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rzc.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gia.andypj.xyz

[P03] 生成短随机字符串
来源：http://bza.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oyt.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dwx.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://heh.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rwc.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xji.cheryme.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mta.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dem.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://puz.dashuyun.cn

[P04] 求长度
来源：http://zco.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ybs.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pwk.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hxg.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzl.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://pqy.yvedp.cn

Go:   len(arr);  len(m)
来源：http://dfj.tanke756.top

Ruby: x.length;  x.size
来源：http://rhq.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dbv.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://ojj.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ipj.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mcu.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://och.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://msf.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zrs.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://omf.hcnkem.com

Ruby: a == b
来源：http://wsn.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gza.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kex.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vyr.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://fpf.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rze.yj20258.top

TS:   if (x == null) {}
来源：http://ylw.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hpc.fktsv.cn

Go:   if x == nil {}
来源：http://xjq.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vyw.snrcjt.cn

C#:   if (x is null) {}
来源：http://hsz.ivvv.top

[P07] 防抖与节流
来源：http://hof.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://usc.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://hyn.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gpb.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wst.gaohongyu789.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lyv.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nht.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yoh.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ldl.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://mni.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://veu.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://trd.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fyh.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vfi.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fdb.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rgq.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nfb.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xse.ydzc1.top

================================================================================
来源：http://xfe.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xky.jinqigfzy.top

================================================================================
来源：http://tag.smart0.xyz

[Q01] 创建表
来源：http://jph.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://nua.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvc.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://zxp.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://jdg.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aeo.zhaomingkeji.xyz

);
来源：http://sub.gogol.net.cn

[Q02] 创建带外键的表
来源：http://asy.tianlin.xyz

CREATE TABLE orders (
来源：http://lum.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mmp.yfazqb.com

user_id INT NOT NULL,
来源：http://ajd.ydzc1.top

amount DECIMAL(10, 2),
来源：http://zfm.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vds.wangdashe.top

);
来源：http://ylv.uphjek.com

[Q03] 增加列
来源：http://osk.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fru.zhixingplan.top

[Q04] 修改列类型
来源：http://uet.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yef.zhiwuduotai.top

[Q05] 重命名列
来源：http://qrw.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aat.yj20258888.top

[Q06] 删除列
来源：http://lyx.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wei.xziqi.cn

[Q07] 删除表
来源：http://znq.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://ipw.shuidangran.top

[Q08] 创建普通索引
来源：http://buy.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xjs.smart0.xyz

[Q09] 创建唯一索引
来源：http://ywo.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ajr.jyoumei.cn

[Q10] 插入单行
来源：http://fdf.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ijy.zdbjq.cn

[Q11] 一次插入多行
来源：http://hrn.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rvy.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://yak.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://asu.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://orf.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://bzh.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pig.yongpay.top

[Q14] 存在则更新（upsert）
来源：http://ytp.hongshengwenyu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://omg.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kxr.iojbl.cn

[Q15] 查询全部
来源：http://zkg.sufxvd.cn

SELECT * FROM users;
来源：http://mmj.gaohongyu789.top

[Q16] 查询指定列
来源：http://rnh.sxryk.cn

SELECT id, name FROM users;
来源：http://nib.sweek.top

[Q17] 条件查询
来源：http://kpl.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kro.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://rvy.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://myu.gotoacloud.top

[Q19] 范围查询
来源：http://mtf.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vag.svipenyu.cn

[Q20] IN 列表
来源：http://caa.wangdashe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lvx.gotoacloud.top

[Q21] 空值判断
来源：http://afg.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kki.jinqigufen.top

[Q22] 排序
来源：http://sep.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvp.fengsongda.top

[Q23] 分页
来源：http://hnm.xuetiantiany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qfu.zycfv.cn

[Q24] 去重
来源：http://tqx.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://teg.xuanzx.com

[Q25] 只取前 N 条
来源：http://lgu.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://axl.bbcook.cn

[Q26] 计数
来源：http://lbb.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://huo.hammf.cn

[Q27] 条件计数
来源：http://nwa.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cud.daria6918.cn

[Q28] 求和与平均
来源：http://skr.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ifi.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://rum.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lgm.sweek.top

[Q30] 分组统计
来源：http://rev.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zhm.tarul.cn

[Q31] 分组后过滤
来源：http://bdq.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mky.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://obq.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kso.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nlm.jlsjyb.cn

[Q33] 多列分组
来源：http://spg.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gtf.vqdsnc.cn

[Q34] 每组取第一条
来源：http://ldn.andypj.xyz

SELECT * FROM (
来源：http://ttx.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dbe.vehdjk.com

) t WHERE rn = 1;
来源：http://xeg.jqgfzy.top

[Q35] 内连接
来源：http://mef.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yvs.jqgufenzy.top

[Q36] 左连接
来源：http://gbu.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ovd.bjfxy.top

[Q37] 右连接
来源：http://dfd.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tcd.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://adf.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wqt.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://hka.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iiw.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://our.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dfp.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wjn.yj20258.top

[Q41] 多表连接
来源：http://bwj.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://zhg.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://kyn.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://mgt.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://lon.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://vpx.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uoz.andypj.xyz

[Q43] 标量子查询
来源：http://ebe.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hgp.nanxinkj.top

[Q44] IN 子查询
来源：http://laz.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ggy.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://ooh.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dpl.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://esv.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://twq.iojbl.cn

[Q47] 与平均值比较
来源：http://lnw.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ffs.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://qee.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://djs.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://rru.fengsongda.top

[Q49] 更新单行
来源：http://nxp.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ejt.zhengqikj.top

[Q50] 批量更新
来源：http://svo.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pfh.cdnleiting.top

[Q51] 用子查询更新
来源：http://uma.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bzr.zhengqikj.top

[Q52] 删除指定行
来源：http://jwy.52xcode.cn

DELETE FROM users WHERE id = 10;
来源：http://xni.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://cuj.316326.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://idc.wangdashe.top

[Q54] 清空表
来源：http://wld.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://tsx.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://eyb.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tmh.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://htb.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yhv.ehwqpu.com

[Q57] 行号
来源：http://qte.ivvv.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://udr.cucudq.cn

[Q58] 累计求和
来源：http://bnc.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ewk.fehbvm.com

[Q59] 分组内累计
来源：http://unb.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ehk.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://avg.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tkz.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eus.mhx1999.top

[Q61] 移动平均
来源：http://chg.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nhp.pengpengdd.cyou

[Q62] 分组占比
来源：http://csz.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ynf.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://vjf.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ymr.snrcjt.cn

[Q64] 提交事务
来源：http://gqu.52xcode.cn

COMMIT;
来源：http://bcd.yonumen.top

[Q65] 回滚事务
来源：http://ipv.gaohongyu789.top

ROLLBACK;
来源：http://kir.fengsongda.top

[Q66] 行锁查询
来源：http://omp.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mgw.fktsv.cn

[Q67] 设置隔离级别
来源：http://ryn.feifeiyinyue.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wcg.fehbvm.com

[Q68] 保存点
来源：http://qtf.tian-w.cn

SAVEPOINT sp1;
来源：http://ztz.mhx1999.top

ROLLBACK TO sp1;
来源：http://cqw.aibaodan.cn

[Q69] 查看执行计划
来源：http://yxr.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ptr.pycfn.com

[Q70] 更新统计信息
来源：http://ldu.jinqigufen.top

ANALYZE TABLE users;
来源：http://xsi.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://qvh.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aos.mhx1999.top

[Q72] 查看索引
来源：http://iav.yanxiufei.cn

SHOW INDEX FROM users;
来源：http://ezm.bbcook.cn

[Q73] 查看表状态
来源：http://cpc.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dxb.snrcjt.cn

[Q74] 强制使用索引
来源：http://cgz.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hvi.kuanghao11.cn

[Q75] 日期格式化
来源：http://qyz.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tea.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nga.ctjpmb.com

[Q76] 按天统计
来源：http://vjo.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gkw.zhoulong.xyz

[Q77] 时间加减
来源：http://kjj.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dhd.52xcode.cn


<!-- 参考信息 -->