代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://fjc.shzxlz.cn

Go:   go f()
来源：http://num.dashuyun.cn

Ruby: Thread.new { f }
来源：http://dvs.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://dyv.hfpthk.cn

[O02] 使用线程池
来源：http://cse.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ajc.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rtp.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://lir.tanke756.top

TS:   // worker_threads 线程池
来源：http://pkr.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://mrs.fanxiaobao.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wow.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ulc.xylfe.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://auz.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://vkk.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://elt.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://lgp.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rho.yj20258.top

TS:   // 同 JS
来源：http://ktz.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://agc.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dci.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jly.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://jnf.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://ejr.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://oxa.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gnu.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://oce.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wow.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ttn.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://woc.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://gom.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://gto.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://hsw.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://ygd.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hlf.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://ttg.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://fcv.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iqa.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mdu.guannengcc.top

Ruby: threads.map(&:join)
来源：http://doc.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://thf.feifeiyinyue.top

[O06] 使用进程池
来源：http://ilx.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rwt.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uvg.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://orj.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://kfp.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rvp.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oyu.cdnleiting.top

Ruby: // fork 块
来源：http://mdi.fanxiaobao.xyz

C#:   Parallel.For
来源：http://lnd.vqdsnc.cn

================================================================================
来源：http://nvu.hnxiangtu.top

P. 常用工具函数
来源：http://phd.zdqjudy.top

================================================================================
来源：http://qrz.svipenyu.cn

[P01] 生成 UUID
来源：http://cch.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://bei.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bto.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://utv.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://ulp.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://vfb.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://sye.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://osj.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://vtu.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://fja.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hik.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vyi.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cyi.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hoo.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://isp.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jey.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gkq.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cjm.xinyue.icu

[P03] 生成短随机字符串
来源：http://sew.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tvw.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gdg.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jod.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ouy.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uyt.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gxl.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mat.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vul.uphjek.com

[P04] 求长度
来源：http://kyo.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bod.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oig.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sdq.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://duc.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://rwd.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://zlk.ppjwa.cn

Ruby: x.length;  x.size
来源：http://svy.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lpl.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://nul.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jcd.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jnv.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://izx.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vbl.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://drd.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://avs.feifeiyinyue.top

Ruby: a == b
来源：http://hqx.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nkf.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oom.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ceo.havefunace.top

PHP:  if (empty($x)) {}
来源：http://wid.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fmx.dianchejie.cn

TS:   if (x == null) {}
来源：http://ogx.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nsd.yonumen.top

Go:   if x == nil {}
来源：http://hsr.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://moy.xuanzx.com

C#:   if (x is null) {}
来源：http://vws.jiagoushi.top

[P07] 防抖与节流
来源：http://lbs.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eei.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://rxw.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gvc.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xlo.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://auo.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xlv.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://udb.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bcb.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://ebb.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mwl.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hjq.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ubw.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lkq.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iet.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hbb.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wsy.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://psi.hesvh.cn

================================================================================
来源：http://dgw.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://enb.ydjk.org.cn

================================================================================
来源：http://gkx.sjlbkw.cn

[Q01] 创建表
来源：http://cta.gotoacloud.top

CREATE TABLE users (
来源：http://jfp.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yzu.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://eob.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://ydb.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yeo.yuxming.cn

);
来源：http://kzw.316326.xyz

[Q02] 创建带外键的表
来源：http://hci.316326.xyz

CREATE TABLE orders (
来源：http://cmr.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jww.dianchejie.cn

user_id INT NOT NULL,
来源：http://uoh.tarul.cn

amount DECIMAL(10, 2),
来源：http://bmh.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vvr.bbcook.cn

);
来源：http://wrh.zhoulong.xyz

[Q03] 增加列
来源：http://frf.daria6918.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://znh.nwbrower.top

[Q04] 修改列类型
来源：http://pnz.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gyc.yuxming.cn

[Q05] 重命名列
来源：http://jdj.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eon.xuanzx.com

[Q06] 删除列
来源：http://hhb.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://dpk.daxiang520.top

[Q07] 删除表
来源：http://spt.yvedp.cn

DROP TABLE IF EXISTS orders;
来源：http://ppm.tianlin.xyz

[Q08] 创建普通索引
来源：http://mhq.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://izq.jianghu66.top

[Q09] 创建唯一索引
来源：http://jsy.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://woa.bjfxy.top

[Q10] 插入单行
来源：http://yaw.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jep.jiagoushi.top

[Q11] 一次插入多行
来源：http://vlv.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uqi.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://oze.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://zxl.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vjc.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://fkq.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jml.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://uhk.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://evr.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://txs.hammf.cn

[Q15] 查询全部
来源：http://dbs.redwolf501.top

SELECT * FROM users;
来源：http://wie.daria6918.cn

[Q16] 查询指定列
来源：http://jrs.yj20258888.top

SELECT id, name FROM users;
来源：http://zsl.snrcjt.cn

[Q17] 条件查询
来源：http://vpe.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mbv.cdnleiting.top

[Q18] 模糊匹配
来源：http://jjt.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://frz.guowangkeji.top

[Q19] 范围查询
来源：http://lrp.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sil.hammf.cn

[Q20] IN 列表
来源：http://ktn.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xul.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://qwh.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zdp.yonumen.top

[Q22] 排序
来源：http://bna.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mxo.yj202588.top

[Q23] 分页
来源：http://qzq.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nhf.fanxiaobao.xyz

[Q24] 去重
来源：http://izy.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://wox.sufxvd.cn

[Q25] 只取前 N 条
来源：http://vel.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hjv.shangyingyoupin.top

[Q26] 计数
来源：http://wfp.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://urm.zhongyouzk.top

[Q27] 条件计数
来源：http://zpr.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xnl.nanxinkj.top

[Q28] 求和与平均
来源：http://szv.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eny.jinyuanbaomall.cn

[Q29] 最大最小值
来源：http://ohh.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tsy.snrcjt.cn

[Q30] 分组统计
来源：http://gmz.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qsn.havefunace.top

[Q31] 分组后过滤
来源：http://fce.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wcq.guannengcc.top

[Q32] 分组拼接字符串
来源：http://ueu.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://phx.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kbk.dianchejie.cn

[Q33] 多列分组
来源：http://ncr.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gwz.zhixingplan.top

[Q34] 每组取第一条
来源：http://xpl.tianlin.xyz

SELECT * FROM (
来源：http://vhj.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://urp.ivvv.top

) t WHERE rn = 1;
来源：http://ygo.cqqwz.cn

[Q35] 内连接
来源：http://nqc.sysykeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uwn.xinyue.icu

[Q36] 左连接
来源：http://htf.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pfs.52xcode.cn

[Q37] 右连接
来源：http://eqy.sxryk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nwv.yueranfly.top

[Q38] 全外连接（PostgreSQL）
来源：http://yoj.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eoq.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://zfp.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hhx.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://owk.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://szf.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ufb.zhongyouzk.top

[Q41] 多表连接
来源：http://jat.hesvh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yep.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://kmp.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://thr.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://tuq.hfpthk.cn

SELECT u.name, o.amount FROM users u
来源：http://adq.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pcq.andypj.xyz

[Q43] 标量子查询
来源：http://ggo.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://arf.haohaochexian.top

[Q44] IN 子查询
来源：http://axq.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ubd.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://zxi.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pes.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sxk.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rgp.pycfn.com

[Q47] 与平均值比较
来源：http://zxz.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jrm.sweek.top

[Q48] CTE 公用表表达式
来源：http://ndt.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vcd.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://ocz.quarkkingdee.top

[Q49] 更新单行
来源：http://nlz.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://upj.ydjk.org.cn

[Q50] 批量更新
来源：http://pzg.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hlt.hesvh.cn

[Q51] 用子查询更新
来源：http://cph.316326.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zcc.pengpengdd.cyou

[Q52] 删除指定行
来源：http://ceq.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://gro.tanke756.top

[Q53] 按条件删除
来源：http://xhh.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ufl.vehdjk.com

[Q54] 清空表
来源：http://ulc.yfazqb.com

TRUNCATE TABLE logs;
来源：http://bbv.epnwcf.com

[Q55] 排名（并列占位）
来源：http://hld.shanyushiyangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uft.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://otx.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sts.zhijiandao.cn

[Q57] 行号
来源：http://hxe.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dlb.quarkkingdee.top

[Q58] 累计求和
来源：http://ohr.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mrg.guannengcc.top

[Q59] 分组内累计
来源：http://xec.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vht.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://wxc.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hvv.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mwg.guowangkeji.top

[Q61] 移动平均
来源：http://pjs.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tta.jqgfzy.top

[Q62] 分组占比
来源：http://wxt.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zqv.zycfv.cn

[Q63] 开启事务
来源：http://lqk.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ptz.svipenyu.cn

[Q64] 提交事务
来源：http://ire.dashuyun.cn

COMMIT;
来源：http://thf.fengsongda.top

[Q65] 回滚事务
来源：http://djn.nanxinkj.top

ROLLBACK;
来源：http://fpd.meibo888.top

[Q66] 行锁查询
来源：http://hui.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jiv.bjfxy.top

[Q67] 设置隔离级别
来源：http://vsb.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qah.yvedp.cn

[Q68] 保存点
来源：http://hxm.0kj1m.cn

SAVEPOINT sp1;
来源：http://xoo.tianlin.xyz

ROLLBACK TO sp1;
来源：http://pxi.daxiang520.top

[Q69] 查看执行计划
来源：http://thc.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://stq.hnqzz.top

[Q70] 更新统计信息
来源：http://vrg.gotoacloud.top

ANALYZE TABLE users;
来源：http://llc.zhoulong.xyz

[Q71] 查看建表语句
来源：http://gnt.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vra.yongpay.top

[Q72] 查看索引
来源：http://eaf.0kj1m.cn

SHOW INDEX FROM users;
来源：http://ede.zhengqikj.top

[Q73] 查看表状态
来源：http://qxn.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nxr.redwolf501.top

[Q74] 强制使用索引
来源：http://clv.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ref.tarul.cn

[Q75] 日期格式化
来源：http://ygp.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zew.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cfg.yonumen.top


<!-- 参考信息 -->