代发 wailian999

================================================================================
来源：http://opl.vehdjk.com

O. 并发与异步
来源：http://lxv.nanxuanxn.top

================================================================================
来源：http://bcl.vehdjk.com

[O01] 启动一个线程
来源：http://swl.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tlv.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tqf.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ejy.zhixingplan.top

TS:   // 同 JS
来源：http://qxu.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://obw.xuanzx.com

Go:   go f()
来源：http://gce.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://gas.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://yag.guowangkeji.top

[O02] 使用线程池
来源：http://tpd.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vaf.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ucg.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://ntb.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://wba.wangdashe.top

Java: Executors.newFixedThreadPool(4)
来源：http://wgk.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ztf.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fkm.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://giy.dianchejie.cn

[O03] 加锁保护共享数据
来源：http://rth.ctjpmb.com

Py:   with lock: shared += 1
来源：http://vso.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://nvi.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zil.gzhubu.top

TS:   // 同 JS
来源：http://jri.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://wkk.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fcd.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fzh.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://iux.redwolf501.top

[O04] 定义异步函数并等待
来源：http://xho.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://qqo.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mcj.xuanzx.com

JS:   async function f() { await g(); }
来源：http://yvc.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kjm.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cgm.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kur.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ltp.yongpay.top

C#:   async Task F() { await G(); }
来源：http://qri.sweek.top

[O05] 并发执行并等待全部完成
来源：http://hzk.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://gwr.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gay.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://adn.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://upv.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xrs.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wiq.cucudq.cn

Ruby: threads.map(&:join)
来源：http://vle.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fat.zhoulong.xyz

[O06] 使用进程池
来源：http://yzz.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xrv.epnwcf.com

PHP:  // pcntl_fork 或多进程队列
来源：http://nqg.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://wkm.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://xmh.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://roy.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gwv.jinghuilouyu.cn

Ruby: // fork 块
来源：http://mct.ppjwa.cn

C#:   Parallel.For
来源：http://kgl.cheryme.top

================================================================================
来源：http://odi.zycfv.cn

P. 常用工具函数
来源：http://qly.c1oappe.top

================================================================================
来源：http://ahl.wangshuangyany.cn

[P01] 生成 UUID
来源：http://kqx.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://xbz.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ibh.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://ssv.iojbl.cn

TS:   crypto.randomUUID()
来源：http://zih.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://jlj.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://bko.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://wlr.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://bxb.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://hys.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ytl.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://nox.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mhy.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xpx.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lsa.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sjn.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sju.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ivd.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://nku.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jej.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wov.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jii.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ecx.tian-w.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ofa.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eph.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tcf.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ipx.xziqi.cn

[P04] 求长度
来源：http://nxb.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wmt.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mpf.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ofi.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cen.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://asf.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://vls.gogol.net.cn

Ruby: x.length;  x.size
来源：http://van.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qgk.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://gaz.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://zve.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zjb.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ryl.dashuyun.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://byq.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gdw.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sib.xinyue.icu

Ruby: a == b
来源：http://hmy.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://twf.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tyc.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tqk.yj202588.top

PHP:  if (empty($x)) {}
来源：http://dzi.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pfk.smart0.xyz

TS:   if (x == null) {}
来源：http://fhn.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ofk.jinqigufen.top

Go:   if x == nil {}
来源：http://ois.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cel.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://kij.fzhhl.top

[P07] 防抖与节流
来源：http://nun.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://agl.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://mwx.uphjek.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aap.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://osi.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://toi.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://isy.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ekn.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kbc.0kj1m.cn

[P08] 处理浮点精度问题
来源：http://ome.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kuc.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gkz.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mpn.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fek.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vxd.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://khc.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sbe.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tsc.ywan-chungtsiang.top

================================================================================
来源：http://gjc.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jip.hcnkem.com

================================================================================
来源：http://cgm.zhixingplan.top

[Q01] 创建表
来源：http://dhe.shanyushiyangtech.top

CREATE TABLE users (
来源：http://fse.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://evn.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://wpl.pengpengdd.cyou

email VARCHAR(100) UNIQUE,
来源：http://zzv.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lqf.havefunace.top

);
来源：http://nmg.pycfn.com

[Q02] 创建带外键的表
来源：http://vrc.pengpengdd.cyou

CREATE TABLE orders (
来源：http://omr.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ghp.nanxuanxn.top

user_id INT NOT NULL,
来源：http://vpx.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://pzu.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://amm.andypj.xyz

);
来源：http://qmi.vqdsnc.cn

[Q03] 增加列
来源：http://zid.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gik.c1oappe.top

[Q04] 修改列类型
来源：http://knd.yj20258888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pxb.jqgfzy.top

[Q05] 重命名列
来源：http://kaq.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qnk.cqqwz.cn

[Q06] 删除列
来源：http://kbs.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://xsn.feifeiyinyue.top

[Q07] 删除表
来源：http://dhz.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://zxf.daria6918.cn

[Q08] 创建普通索引
来源：http://opv.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fgg.hysaishi.cn

[Q09] 创建唯一索引
来源：http://fys.aibaodan.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zuz.9152youxi.cn

[Q10] 插入单行
来源：http://mbv.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://txx.hnqzz.top

[Q11] 一次插入多行
来源：http://kek.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xqm.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://yek.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://emj.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kby.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://rlz.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hid.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://jax.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nzr.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://txg.zdqjudy.top

[Q15] 查询全部
来源：http://nhe.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://aqn.hcnkem.com

[Q16] 查询指定列
来源：http://dtu.sjlbkw.cn

SELECT id, name FROM users;
来源：http://wmr.bjfxy.top

[Q17] 条件查询
来源：http://dwx.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cuc.tian-w.cn

[Q18] 模糊匹配
来源：http://nok.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://utu.cheryme.top

[Q19] 范围查询
来源：http://oak.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kcl.yvedp.cn

[Q20] IN 列表
来源：http://ufr.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lnk.sufxvd.cn

[Q21] 空值判断
来源：http://uob.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://irk.ybcxt.top

[Q22] 排序
来源：http://avo.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nke.hysaishi.cn

[Q23] 分页
来源：http://hyv.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fjv.kuanghao11.cn

[Q24] 去重
来源：http://uph.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://vbr.daxiang520.top

[Q25] 只取前 N 条
来源：http://fnv.cucudq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cum.jiagoushi.top

[Q26] 计数
来源：http://poa.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://thc.ctjpmb.com

[Q27] 条件计数
来源：http://luk.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nvy.quarkkingdee.top

[Q28] 求和与平均
来源：http://rsu.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wzv.xuanzx.com

[Q29] 最大最小值
来源：http://nqy.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uvn.xuanzx.com

[Q30] 分组统计
来源：http://ehc.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://icy.smart0.xyz

[Q31] 分组后过滤
来源：http://qax.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lpn.smart0.xyz

[Q32] 分组拼接字符串
来源：http://wqk.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zcm.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vvu.sxryk.cn

[Q33] 多列分组
来源：http://ltl.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tdq.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://qlj.zhixingplan.top

SELECT * FROM (
来源：http://ggw.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uub.sweek.top

) t WHERE rn = 1;
来源：http://zsp.sxryk.cn

[Q35] 内连接
来源：http://ene.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mzj.tarul.cn

[Q36] 左连接
来源：http://cko.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://koz.nanxinkj.top

[Q37] 右连接
来源：http://hpy.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ryo.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pib.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dhf.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://nzf.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://tmm.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jdb.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yjc.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jla.hnqzz.top

[Q41] 多表连接
来源：http://nsy.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://hml.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://brt.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://pjn.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://xzg.guannengcc.top

SELECT u.name, o.amount FROM users u
来源：http://wsy.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rum.ehwqpu.com

[Q43] 标量子查询
来源：http://jjt.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cid.jinqigfzy.top

[Q44] IN 子查询
来源：http://xrw.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qkb.bbcook.cn

[Q45] EXISTS 判断存在
来源：http://dwt.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://izj.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iqr.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ibg.daria6918.cn

[Q47] 与平均值比较
来源：http://zfs.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fae.pycfn.com

[Q48] CTE 公用表表达式
来源：http://cis.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oca.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://ptt.0kj1m.cn

[Q49] 更新单行
来源：http://clu.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rmv.hfpthk.cn

[Q50] 批量更新
来源：http://lew.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://azm.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://nuk.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uku.epnwcf.com

[Q52] 删除指定行
来源：http://cwd.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://byp.zhiwuduotai.top

[Q53] 按条件删除
来源：http://xti.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://taz.guannengcc.top

[Q54] 清空表
来源：http://orc.bjfxy.top

TRUNCATE TABLE logs;
来源：http://pnq.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://ago.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nts.nwbrower.top

[Q56] 密集排名（并列不占位）
来源：http://dig.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uii.jiagoushi.top

[Q57] 行号
来源：http://nat.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uiw.cqqwz.cn

[Q58] 累计求和
来源：http://bqx.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mgw.yueranfly.top

[Q59] 分组内累计
来源：http://zcl.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://drr.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://ksc.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pnq.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://djo.birdmap.top

[Q61] 移动平均
来源：http://lta.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rap.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://uzu.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bbt.hongshengwenyu.top

[Q63] 开启事务
来源：http://hde.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zjn.shanyushiyangtech.top

[Q64] 提交事务
来源：http://fey.ywan-chungtsiang.top

COMMIT;
来源：http://jtj.sysykeji.top

[Q65] 回滚事务
来源：http://tmq.sysykeji.top

ROLLBACK;
来源：http://tmg.yangfankeji.com

[Q66] 行锁查询
来源：http://rro.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hta.tian-w.cn

[Q67] 设置隔离级别
来源：http://yvl.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tnn.zdbjq.cn

[Q68] 保存点
来源：http://pzr.daria6918.cn

SAVEPOINT sp1;
来源：http://klc.chenlongwang.top

ROLLBACK TO sp1;
来源：http://awv.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://tvg.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mgu.hammf.cn

[Q70] 更新统计信息
来源：http://nwt.zhongyouzk.top

ANALYZE TABLE users;
来源：http://bqd.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://ozb.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dbd.redwolf501.top

[Q72] 查看索引
来源：http://ebe.52xcode.cn


<!-- 参考信息 -->