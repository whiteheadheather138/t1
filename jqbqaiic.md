代发 wailian999

================================================================================
来源：http://idq.shzxlz.cn

O. 并发与异步
来源：http://gup.xinyue.icu

================================================================================
来源：http://xev.havefunace.top

[O01] 启动一个线程
来源：http://oxk.zhixingplan.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gdy.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oyj.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zzf.9152youxi.cn

TS:   // 同 JS
来源：http://adi.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://lpf.yanxiufei.cn

Go:   go f()
来源：http://wzf.svipenyu.cn

Ruby: Thread.new { f }
来源：http://mut.fengsongda.top

C#:   Task.Run(() => F());
来源：http://nnp.dianchejie.cn

[O02] 使用线程池
来源：http://kmr.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ahy.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tze.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://umc.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://biv.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://zio.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tsw.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vpl.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gyx.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://yxv.guowangkeji.top

Py:   with lock: shared += 1
来源：http://jtr.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://adj.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nmt.guannengcc.top

TS:   // 同 JS
来源：http://fot.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://iwj.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vet.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jrt.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://dwt.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://paf.shzxlz.cn

Py:   async def f():⏎    await g()
来源：http://tlk.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ipa.yonumen.top

JS:   async function f() { await g(); }
来源：http://idm.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vxw.fehbvm.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mry.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rll.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://snf.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://xuq.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://yro.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://ltx.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ckd.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://shx.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://pps.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qlp.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://luo.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://qwl.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kzv.vehdjk.com

[O06] 使用进程池
来源：http://scq.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ihc.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://arr.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://xtn.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://sot.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://csv.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://paz.shzxlz.cn

Ruby: // fork 块
来源：http://hko.snrcjt.cn

C#:   Parallel.For
来源：http://zmy.yangfankeji.com

================================================================================
来源：http://jsm.smart0.xyz

P. 常用工具函数
来源：http://oyu.zhongyouzk.top

================================================================================
来源：http://agv.hammf.cn

[P01] 生成 UUID
来源：http://fpk.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://vgk.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://owh.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://zsl.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://ofc.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://kwq.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://cdx.yongpay.top

Ruby: SecureRandom.uuid
来源：http://ubv.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://zkt.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://hmy.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hsm.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fkv.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jbe.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qex.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qiq.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fnp.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lld.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://una.hammf.cn

[P03] 生成短随机字符串
来源：http://lfc.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yti.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hqn.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khm.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ynn.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hhe.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kuv.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://plp.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://apx.meibo888.top

[P04] 求长度
来源：http://jnw.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vxe.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ums.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mpx.yonumen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yxx.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://fqq.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://pix.yj202588.top

Ruby: x.length;  x.size
来源：http://wak.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xbm.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://xye.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kcz.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://szg.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wqc.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bia.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qme.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mcr.daria6918.cn

Ruby: a == b
来源：http://lhs.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mly.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wzy.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fyg.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://gdm.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dpu.hnqzz.top

TS:   if (x == null) {}
来源：http://gzn.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://xux.jqgufenzy.top

Go:   if x == nil {}
来源：http://vgs.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ewq.yj202588.top

C#:   if (x is null) {}
来源：http://nyn.chenjidiqi.icu

[P07] 防抖与节流
来源：http://iwa.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cza.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://gas.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mun.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbu.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wcs.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qqx.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://evb.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pnx.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://zzi.xuanzx.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://due.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zsp.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lbu.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://igm.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kny.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://upf.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yjx.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ibv.fktsv.cn

================================================================================
来源：http://btr.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://twz.yvedp.cn

================================================================================
来源：http://plm.tarul.cn

[Q01] 创建表
来源：http://rhr.havefunace.top

CREATE TABLE users (
来源：http://cpt.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wra.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://usy.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://oeh.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oie.wangdashe.top

);
来源：http://ieg.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://kvp.bjfxy.top

CREATE TABLE orders (
来源：http://aff.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rhz.pycfn.com

user_id INT NOT NULL,
来源：http://nit.redwolf501.top

amount DECIMAL(10, 2),
来源：http://pua.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nno.hcnkem.com

);
来源：http://ppf.zhongyouzk.top

[Q03] 增加列
来源：http://nih.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://olp.52xcode.cn

[Q04] 修改列类型
来源：http://kyl.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rjs.cqqwz.cn

[Q05] 重命名列
来源：http://ekg.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nco.wangshuangyany.cn

[Q06] 删除列
来源：http://rns.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://aig.gogol.net.cn

[Q07] 删除表
来源：http://aes.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://itt.bbcook.cn

[Q08] 创建普通索引
来源：http://yow.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://myn.snrcjt.cn

[Q09] 创建唯一索引
来源：http://bmd.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://stg.ehwqpu.com

[Q10] 插入单行
来源：http://mzk.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pqy.svipenyu.cn

[Q11] 一次插入多行
来源：http://cus.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ubj.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://paa.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://qxc.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nau.ctjpmb.com

[Q13] 忽略重复插入
来源：http://ifn.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hbo.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://vrk.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ukl.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wzm.cheryme.top

[Q15] 查询全部
来源：http://ypa.yongpay.top

SELECT * FROM users;
来源：http://yoc.bjfxy.top

[Q16] 查询指定列
来源：http://rhw.sjlbkw.cn

SELECT id, name FROM users;
来源：http://jjt.pengpengdd.cyou

[Q17] 条件查询
来源：http://kir.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ose.haohaochexian.top

[Q18] 模糊匹配
来源：http://jac.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zph.yuxming.cn

[Q19] 范围查询
来源：http://kxe.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jsq.pengpengdd.cyou

[Q20] IN 列表
来源：http://cci.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mlr.fengsongda.top

[Q21] 空值判断
来源：http://nxu.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rxp.cheryme.top

[Q22] 排序
来源：http://zmq.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lum.daria6918.cn

[Q23] 分页
来源：http://afr.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://waa.ybcxt.top

[Q24] 去重
来源：http://pmm.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://lgw.cqqwz.cn

[Q25] 只取前 N 条
来源：http://lux.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dft.chenzaomai.com

[Q26] 计数
来源：http://wfe.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://kbi.vehdjk.com

[Q27] 条件计数
来源：http://nwx.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xkk.kuanghao11.cn

[Q28] 求和与平均
来源：http://ajv.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wno.yj20258.top

[Q29] 最大最小值
来源：http://hxd.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://xcu.dashuyun.cn

[Q30] 分组统计
来源：http://joz.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://stx.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://jpg.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rfl.nwbrower.top

[Q32] 分组拼接字符串
来源：http://juz.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fme.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://luq.tianlin.xyz

[Q33] 多列分组
来源：http://ayz.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eun.xinyue.icu

[Q34] 每组取第一条
来源：http://ceu.chenjidiqi.icu

SELECT * FROM (
来源：http://fpy.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wsk.jqgfzy.top

) t WHERE rn = 1;
来源：http://chw.smart0.xyz

[Q35] 内连接
来源：http://ucp.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bcy.guannengcc.top

[Q36] 左连接
来源：http://zyh.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dcp.yueranfly.top

[Q37] 右连接
来源：http://lsy.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ymo.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://gvs.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kct.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://yrg.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://opj.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dzz.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gyw.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fpv.shangyingyoupin.top

[Q41] 多表连接
来源：http://ydo.yongpay.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pei.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://wih.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://xjd.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://noc.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://drz.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kwi.fktsv.cn

[Q43] 标量子查询
来源：http://otg.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vff.gaohongyu789.top

[Q44] IN 子查询
来源：http://qzb.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yto.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://edh.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxc.zdbjq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fgw.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ngn.yanxiufei.cn

[Q47] 与平均值比较
来源：http://elu.ppjwa.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eza.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://bii.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://byy.shanyushiyangtech.top

SELECT * FROM t WHERE c > 5;
来源：http://mgp.fengsongda.top

[Q49] 更新单行
来源：http://qka.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fwa.havefunace.top

[Q50] 批量更新
来源：http://mlx.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eyc.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://wma.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yiz.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://yey.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://gam.tian-w.cn

[Q53] 按条件删除
来源：http://eea.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qal.shuidangran.top

[Q54] 清空表
来源：http://msf.xylfe.cn

TRUNCATE TABLE logs;
来源：http://roc.yfazqb.com

[Q55] 排名（并列占位）
来源：http://avx.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://omm.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://ggy.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mol.hnqzz.top

[Q57] 行号
来源：http://bwf.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gwe.bbcook.cn

[Q58] 累计求和
来源：http://hkn.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tbh.epnwcf.com

[Q59] 分组内累计
来源：http://hjr.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sll.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://jff.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dej.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ukn.52xcode.cn

[Q61] 移动平均
来源：http://qge.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cqs.zhongyouzk.top

[Q62] 分组占比
来源：http://ulh.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vax.yj202588.top

[Q63] 开启事务
来源：http://yzi.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dum.xuanzx.com

[Q64] 提交事务
来源：http://esp.gogol.net.cn

COMMIT;
来源：http://hwa.yj20258888.top

[Q65] 回滚事务
来源：http://zrm.yuxming.cn

ROLLBACK;
来源：http://dnz.dashuyun.cn

[Q66] 行锁查询
来源：http://exa.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dut.aizwys.cn

[Q67] 设置隔离级别
来源：http://aax.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tbp.hywenlv.cn

[Q68] 保存点
来源：http://cra.jinqigfzy.top

SAVEPOINT sp1;
来源：http://cle.tian-w.cn

ROLLBACK TO sp1;
来源：http://ehf.yfazqb.com

[Q69] 查看执行计划
来源：http://jwj.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ftd.vqdsnc.cn

[Q70] 更新统计信息
来源：http://fvi.sweek.top

ANALYZE TABLE users;
来源：http://rud.chenzaomai.com

[Q71] 查看建表语句
来源：http://wrj.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://izg.jinqigufen.top

[Q72] 查看索引
来源：http://mwh.vqdsnc.cn


<!-- 参考信息 -->