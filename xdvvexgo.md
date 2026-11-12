代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rlq.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://peg.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yjc.cdnleiting.top

TS:   // 同 JS
来源：http://aso.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://xyk.svipenyu.cn

Go:   go f()
来源：http://ixe.zycfv.cn

Ruby: Thread.new { f }
来源：http://jnw.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://syk.zhixingplan.top

[O02] 使用线程池
来源：http://hqc.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wcg.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zjd.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://fqr.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://fjt.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://xng.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hio.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hdj.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uly.daxiang520.top

[O03] 加锁保护共享数据
来源：http://dmm.hnqzz.top

Py:   with lock: shared += 1
来源：http://vac.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://uaz.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://who.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://lub.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://xjt.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cvh.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kdp.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://cgr.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://szr.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://evl.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qiz.tanke756.top

JS:   async function f() { await g(); }
来源：http://kdg.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://clp.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tmv.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ych.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://okw.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://vxe.cdnleiting.top

[O05] 并发执行并等待全部完成
来源：http://xtg.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://qxf.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lrj.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://xih.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://lub.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wcf.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kmn.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://bei.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://asc.hcnkem.com

[O06] 使用进程池
来源：http://zst.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jul.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://eeg.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://qls.ivvv.top

TS:   // child_process / cluster 模块
来源：http://ueb.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gzp.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gib.tian-w.cn

Ruby: // fork 块
来源：http://kyb.chenzaomai.com

C#:   Parallel.For
来源：http://fjj.cheryme.top

================================================================================
来源：http://xzj.jinqigfzy.top

P. 常用工具函数
来源：http://ecz.birdmap.top

================================================================================
来源：http://hcz.ydzc1.top

[P01] 生成 UUID
来源：http://vdh.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://idu.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mvv.hfpthk.cn

JS:   crypto.randomUUID()
来源：http://whu.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://ylh.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://oqs.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://lis.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://orh.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://cpo.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://ibu.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aug.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://klx.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ssh.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rbc.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://quh.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://deg.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lau.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pan.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://ajk.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://atk.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hzj.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wrn.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://msh.cqqwz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xti.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jjg.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qvm.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dwy.tarul.cn

[P04] 求长度
来源：http://skk.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ltb.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://klz.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tqw.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dts.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://rcx.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://svz.ivvv.top

Ruby: x.length;  x.size
来源：http://qtx.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ayo.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://scr.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kft.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dgq.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yvj.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lzq.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qio.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://jya.hesvh.cn

Ruby: a == b
来源：http://vmq.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://scw.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mcq.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fuu.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://sax.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ibw.yuxming.cn

TS:   if (x == null) {}
来源：http://pfu.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qwh.tian-w.cn

Go:   if x == nil {}
来源：http://kwq.jinqigfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sdl.fzhhl.top

C#:   if (x is null) {}
来源：http://ewb.quarkkingdee.top

[P07] 防抖与节流
来源：http://ofd.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ase.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://wcd.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pwj.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aju.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jfn.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hpd.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rld.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tad.xylfe.cn

[P08] 处理浮点精度问题
来源：http://aut.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ddb.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://koo.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zly.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bbc.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vcu.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lhi.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bgg.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://evm.zhijiandao.cn

================================================================================
来源：http://vom.zdbjq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mzx.zycfv.cn

================================================================================
来源：http://btw.52xcode.cn

[Q01] 创建表
来源：http://njt.cqqwz.cn

CREATE TABLE users (
来源：http://nhv.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gcl.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://ngi.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://ini.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://klc.hnxiangtu.top

);
来源：http://vhp.chenlongwang.top

[Q02] 创建带外键的表
来源：http://fzf.zhixingplan.top

CREATE TABLE orders (
来源：http://bfv.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nxn.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://ksg.316326.xyz

amount DECIMAL(10, 2),
来源：http://ynp.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zsh.shanyushiyangkeji.top

);
来源：http://fda.ctjpmb.com

[Q03] 增加列
来源：http://tdj.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zea.hnqzz.top

[Q04] 修改列类型
来源：http://sfj.nwbrower.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rab.jinqigufen.top

[Q05] 重命名列
来源：http://rie.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dzf.shanyushiyangkeji.top

[Q06] 删除列
来源：http://pfx.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://cfv.hcnkem.com

[Q07] 删除表
来源：http://uzl.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://wgc.jinqigufen.top

[Q08] 创建普通索引
来源：http://aru.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://abc.fzhhl.top

[Q09] 创建唯一索引
来源：http://fbv.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mgb.yonumen.top

[Q10] 插入单行
来源：http://nix.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ogv.guannengcc.top

[Q11] 一次插入多行
来源：http://snn.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uio.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://dxj.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://opx.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zxo.svipenyu.cn

[Q13] 忽略重复插入
来源：http://guj.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dol.tian-w.cn

[Q14] 存在则更新（upsert）
来源：http://aok.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gdp.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zqf.zhengqikj.top

[Q15] 查询全部
来源：http://egx.jqgufenzy.top

SELECT * FROM users;
来源：http://dxb.xylfe.cn

[Q16] 查询指定列
来源：http://xiz.hnxiangtu.top

SELECT id, name FROM users;
来源：http://prg.cashguo.top

[Q17] 条件查询
来源：http://cvg.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hgm.yfazqb.com

[Q18] 模糊匹配
来源：http://yjy.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jpk.xziqi.cn

[Q19] 范围查询
来源：http://kvu.dianchejie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://efu.shangyingyoupin.top

[Q20] IN 列表
来源：http://utg.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vkg.nanxuanxn.top

[Q21] 空值判断
来源：http://kdt.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lki.52xcode.cn

[Q22] 排序
来源：http://usk.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dho.gogol.net.cn

[Q23] 分页
来源：http://oev.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dre.jinqigfzy.top

[Q24] 去重
来源：http://yti.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://hyn.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://yir.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xmt.fzhhl.top

[Q26] 计数
来源：http://crv.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://hzd.tian-w.cn

[Q27] 条件计数
来源：http://yql.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zcj.zhengqikj.top

[Q28] 求和与平均
来源：http://sha.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mxt.fehbvm.com

[Q29] 最大最小值
来源：http://zja.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oxi.gzhubu.top

[Q30] 分组统计
来源：http://jjm.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dcl.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://zrw.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iot.52xcode.cn

[Q32] 分组拼接字符串
来源：http://dqt.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xpd.xziqi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sfr.pycfn.com

[Q33] 多列分组
来源：http://odq.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://voz.hysaishi.cn

[Q34] 每组取第一条
来源：http://mez.yanxiufei.cn

SELECT * FROM (
来源：http://dzo.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mlh.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://for.sufxvd.cn

[Q35] 内连接
来源：http://kyb.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lvy.hnxiangtu.top

[Q36] 左连接
来源：http://gib.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rnd.snrcjt.cn

[Q37] 右连接
来源：http://ytz.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://btm.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wdn.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kuj.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://iho.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oln.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://imf.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cru.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://shf.wangshuangyany.cn

[Q41] 多表连接
来源：http://tfu.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://ear.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://lyi.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://qpl.meibo888.top

[Q42] 连接条件附加过滤
来源：http://oqr.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://kul.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wka.shuidangran.top

[Q43] 标量子查询
来源：http://dgc.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fgp.fzhhl.top

[Q44] IN 子查询
来源：http://pyy.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hjy.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://ehc.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dfb.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://jkx.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ezl.vqdsnc.cn

[Q47] 与平均值比较
来源：http://dop.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://htk.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://tko.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qqi.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://tep.ivvv.top

[Q49] 更新单行
来源：http://lsc.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://poy.epnwcf.com

[Q50] 批量更新
来源：http://box.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://loc.xinyue.icu

[Q51] 用子查询更新
来源：http://deg.yuanzhike.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cjm.ivvv.top

[Q52] 删除指定行
来源：http://ucg.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://zmz.jinqigfzy.top

[Q53] 按条件删除
来源：http://zlg.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zxy.fehbvm.com

[Q54] 清空表
来源：http://vwx.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://fmr.mhx1999.top

[Q55] 排名（并列占位）
来源：http://czf.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wwz.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://bhq.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xed.zhaomingkeji.xyz

[Q57] 行号
来源：http://ont.jlsjyb.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://znd.tian-w.cn

[Q58] 累计求和
来源：http://byo.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://utp.yvedp.cn

[Q59] 分组内累计
来源：http://dkz.9152youxi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mvz.bbcook.cn

[Q60] 取上一行 / 下一行
来源：http://blg.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jrx.tian-w.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ccb.gogol.net.cn

[Q61] 移动平均
来源：http://vjo.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jjp.snrcjt.cn

[Q62] 分组占比
来源：http://sdh.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jds.nanxinkj.top

[Q63] 开启事务
来源：http://ovd.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kia.zhaomingkeji.xyz

[Q64] 提交事务
来源：http://occ.zycfv.cn

COMMIT;
来源：http://uac.fktsv.cn

[Q65] 回滚事务
来源：http://avl.aizwys.cn

ROLLBACK;
来源：http://bqy.jinyuanbaomall.cn

[Q66] 行锁查询
来源：http://phd.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iex.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://scq.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://enc.ppjwa.cn

[Q68] 保存点
来源：http://fkh.hammf.cn

SAVEPOINT sp1;
来源：http://nrc.ppjwa.cn

ROLLBACK TO sp1;
来源：http://roh.hnqzz.top

[Q69] 查看执行计划
来源：http://qds.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tfs.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://yeo.shuidangran.top

ANALYZE TABLE users;
来源：http://ahj.havefunace.top

[Q71] 查看建表语句
来源：http://bvt.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://olc.hammf.cn

[Q72] 查看索引
来源：http://blj.tian-w.cn

SHOW INDEX FROM users;
来源：http://pbd.cucudq.cn

[Q73] 查看表状态
来源：http://ulm.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uda.fzhhl.top

[Q74] 强制使用索引
来源：http://msj.zhoulong.xyz


<!-- 参考信息 -->