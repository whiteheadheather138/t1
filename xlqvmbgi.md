代发 wailian999

[O02] 使用线程池
来源：http://gnr.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vpg.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://spd.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://odk.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://rwp.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://drj.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://afq.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mzi.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ixl.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://myc.cheryme.top

Py:   with lock: shared += 1
来源：http://tfa.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fwy.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gdz.yj202588.top

TS:   // 同 JS
来源：http://nsd.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://yvy.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yel.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://akq.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://gqz.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://ohu.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://pbq.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://onx.zycfv.cn

JS:   async function f() { await g(); }
来源：http://dne.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://gfc.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bno.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mic.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://ceb.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://sek.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://sfc.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://szd.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vmv.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://mlh.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://fhg.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lml.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://swe.epnwcf.com

Ruby: threads.map(&:join)
来源：http://hgq.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://swe.gaohongyu789.top

[O06] 使用进程池
来源：http://gdv.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hgz.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zjg.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://bnj.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://oqj.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://soh.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bax.zycfv.cn

Ruby: // fork 块
来源：http://vdq.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://bay.uphjek.com

================================================================================
来源：http://yfi.yonumen.top

P. 常用工具函数
来源：http://dog.0kj1m.cn

================================================================================
来源：http://euq.bjfxy.top

[P01] 生成 UUID
来源：http://rjz.havefunace.top

Py:   str(uuid.uuid4())
来源：http://ttq.gogol.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kzd.xziqi.cn

JS:   crypto.randomUUID()
来源：http://yhb.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://nmo.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://tnt.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://qnu.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://qyi.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://hir.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://vws.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iph.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uxv.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gea.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xtn.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://olu.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fzr.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wea.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sdq.iojbl.cn

[P03] 生成短随机字符串
来源：http://ywd.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://umn.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vnn.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wfg.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mku.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bzj.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fsu.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mkx.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cdw.hesvh.cn

[P04] 求长度
来源：http://fdm.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ctd.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://voe.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bwu.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wqw.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://mdb.bbcook.cn

Go:   len(arr);  len(m)
来源：http://umd.havefunace.top

Ruby: x.length;  x.size
来源：http://xpw.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://krn.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://tzn.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://uqe.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jka.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cao.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pnd.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ska.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wau.nanxuanxn.top

Ruby: a == b
来源：http://pxx.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rxp.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rdf.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://por.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://bcv.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://haa.sjlbkw.cn

TS:   if (x == null) {}
来源：http://aau.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wvj.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://dva.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sqr.316326.xyz

C#:   if (x is null) {}
来源：http://bby.chenlongwang.top

[P07] 防抖与节流
来源：http://uqd.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xmg.havefunace.top

PHP:  // 手写时间戳比较
来源：http://swm.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xzp.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zow.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iba.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mia.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://fpz.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://miv.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://hmw.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zxe.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nhr.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://coi.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mro.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dsv.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pbt.hfpthk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bxg.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://utm.fengsongda.top

================================================================================
来源：http://eyw.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zsv.sweek.top

================================================================================
来源：http://ldg.meibo888.top

[Q01] 创建表
来源：http://nmm.fengsongda.top

CREATE TABLE users (
来源：http://ymm.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kux.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://miv.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://oli.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xuy.hnxiangtu.top

);
来源：http://zbb.jianghu66.top

[Q02] 创建带外键的表
来源：http://ygn.pengpengdd.cyou

CREATE TABLE orders (
来源：http://sho.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://llr.fanxiaobao.xyz

user_id INT NOT NULL,
来源：http://gex.zycfv.cn

amount DECIMAL(10, 2),
来源：http://ilc.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oir.fengsongda.top

);
来源：http://ucd.xylfe.cn

[Q03] 增加列
来源：http://mmx.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ryv.xuetiantiany.cn

[Q04] 修改列类型
来源：http://hkn.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ote.wangshuangyany.cn

[Q05] 重命名列
来源：http://irb.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wee.ywan-chungtsiang.top

[Q06] 删除列
来源：http://uhd.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://xdx.daxiang520.top

[Q07] 删除表
来源：http://ytf.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://nqj.gzhubu.top

[Q08] 创建普通索引
来源：http://mwa.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ttx.tarul.cn

[Q09] 创建唯一索引
来源：http://saf.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sda.nwbrower.top

[Q10] 插入单行
来源：http://kqe.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kux.yongpay.top

[Q11] 一次插入多行
来源：http://cwm.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kry.xingfuxueyuan.xyz

[Q12] 插入后取自增 ID
来源：http://taf.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://bxz.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cqo.hywenlv.cn

[Q13] 忽略重复插入
来源：http://myk.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aas.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://rqz.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cho.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vcc.chenlongwang.top

[Q15] 查询全部
来源：http://soz.nwbrower.top

SELECT * FROM users;
来源：http://ovc.yj202588.top

[Q16] 查询指定列
来源：http://aeu.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://vnu.wangdashe.top

[Q17] 条件查询
来源：http://ljv.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://enn.gaohongyu789.top

[Q18] 模糊匹配
来源：http://hir.quarkkingdee.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wfj.jinqigufen.top

[Q19] 范围查询
来源：http://gje.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dnx.jinqigufen.top

[Q20] IN 列表
来源：http://wro.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tnh.andypj.xyz

[Q21] 空值判断
来源：http://qox.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dop.xuetiantiany.cn

[Q22] 排序
来源：http://ltc.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xyg.havefunace.top

[Q23] 分页
来源：http://nye.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jdm.fehbvm.com

[Q24] 去重
来源：http://taf.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://vkp.yj20258888.top

[Q25] 只取前 N 条
来源：http://eai.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://exi.aibaodan.cn

[Q26] 计数
来源：http://itp.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://vhh.gogol.net.cn

[Q27] 条件计数
来源：http://dri.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uhg.0kj1m.cn

[Q28] 求和与平均
来源：http://yvu.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qjx.ivvv.top

[Q29] 最大最小值
来源：http://exa.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ror.chenlongwang.top

[Q30] 分组统计
来源：http://pzk.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nlf.0kj1m.cn

[Q31] 分组后过滤
来源：http://tsn.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nug.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://rrq.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ewy.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bpk.hongshengwenyu.top

[Q33] 多列分组
来源：http://zwh.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://itd.jqgufenzy.top

[Q34] 每组取第一条
来源：http://fbh.hnqzz.top

SELECT * FROM (
来源：http://bet.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yfy.hfpthk.cn

) t WHERE rn = 1;
来源：http://hrm.chenzaomai.com

[Q35] 内连接
来源：http://spv.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lkc.zdqjudy.top

[Q36] 左连接
来源：http://wuo.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qhs.yanxiufei.cn

[Q37] 右连接
来源：http://trd.fanxiaobao.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xms.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://lbj.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cmt.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://nui.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dxq.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://szw.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ebn.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://duv.kuanghao11.cn

[Q41] 多表连接
来源：http://que.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ndj.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://rjl.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://ynd.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://tay.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://ygc.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jqf.aizwys.cn

[Q43] 标量子查询
来源：http://dfu.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dgj.gotoacloud.top

[Q44] IN 子查询
来源：http://vby.yuxming.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fmt.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://lib.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxx.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://utw.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nsg.redwolf501.top

[Q47] 与平均值比较
来源：http://evq.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vdi.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://cgy.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ghd.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://fam.aibaodan.cn

[Q49] 更新单行
来源：http://xsn.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wrw.wangshuangyany.cn

[Q50] 批量更新
来源：http://mat.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yki.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://ieb.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://czh.tarul.cn

[Q52] 删除指定行
来源：http://hkf.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://pnx.jiagoushi.top

[Q53] 按条件删除
来源：http://xld.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wnh.tianlin.xyz

[Q54] 清空表
来源：http://gil.dashuyun.cn

TRUNCATE TABLE logs;
来源：http://uas.xuanzx.com

[Q55] 排名（并列占位）
来源：http://vyx.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fsc.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://ssv.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rmk.xuetiantiany.cn

[Q57] 行号
来源：http://zdd.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ywj.xylfe.cn

[Q58] 累计求和
来源：http://pac.cucudq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lih.yanxiufei.cn

[Q59] 分组内累计
来源：http://blt.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lew.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://ezy.guannengcc.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ofn.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://huq.fehbvm.com

[Q61] 移动平均
来源：http://wmj.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://svr.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://zqn.hcnkem.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uay.yuxming.cn

[Q63] 开启事务
来源：http://qac.0kj1m.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mtz.redwolf501.top

[Q64] 提交事务
来源：http://ybi.zhaomingkeji.xyz

COMMIT;
来源：http://vtj.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://vpf.jqgfzy.top

ROLLBACK;
来源：http://rbv.feifeiyinyue.top

[Q66] 行锁查询
来源：http://dlm.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ddb.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://neo.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qnd.haohaochexian.top

[Q68] 保存点
来源：http://tzg.c1oappe.top

SAVEPOINT sp1;
来源：http://olm.yongpay.top

ROLLBACK TO sp1;
来源：http://gko.smart0.xyz

[Q69] 查看执行计划
来源：http://spc.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vuh.uphjek.com

[Q70] 更新统计信息
来源：http://aav.epnwcf.com

ANALYZE TABLE users;
来源：http://yog.yuanzhike.top

[Q71] 查看建表语句
来源：http://pxe.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jkf.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://gxp.fzhhl.top

SHOW INDEX FROM users;
来源：http://ipf.gaohongyu789.top

[Q73] 查看表状态
来源：http://jvn.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tjh.snrcjt.cn

[Q74] 强制使用索引
来源：http://umh.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dsx.316326.xyz

[Q75] 日期格式化
来源：http://kkx.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bxu.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rah.tian-w.cn

[Q76] 按天统计
来源：http://xka.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://awe.ehwqpu.com

[Q77] 时间加减
来源：http://pkq.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://atp.zhixingplan.top


<!-- 参考信息 -->