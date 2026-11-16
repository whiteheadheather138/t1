代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://qmc.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zwz.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://sil.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://krc.yangfankeji.com

PHP:  // 手写递归函数
来源：http://oos.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mqk.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jhh.jqgfzy.top

Java: // 手写递归
来源：http://san.sxryk.cn

Go:   // 手写递归
来源：http://bcy.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fyj.fktsv.cn

C#:   // 手写递归
来源：http://ujb.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rlh.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zfh.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://guh.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ekm.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nfm.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://okk.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aay.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fvq.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://onk.meibo888.top

================================================================================
来源：http://not.316326.xyz

O. 并发与异步
来源：http://emz.hnqzz.top

================================================================================
来源：http://beg.guowangkeji.top

[O01] 启动一个线程
来源：http://fgv.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dlu.iojbl.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mvr.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tca.wangshuangyany.cn

TS:   // 同 JS
来源：http://bje.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://opv.yj20258.top

Go:   go f()
来源：http://zen.nanxinkj.top

Ruby: Thread.new { f }
来源：http://xte.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://xyx.chenzaomai.com

[O02] 使用线程池
来源：http://nyq.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pay.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nhh.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://xan.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://pva.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://cit.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jiy.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uqg.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zpy.redwolf501.top

[O03] 加锁保护共享数据
来源：http://azx.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://tgs.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://suf.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://arj.jiagoushi.top

TS:   // 同 JS
来源：http://lxu.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://vlh.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xiv.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wht.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://zjk.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://saw.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://hry.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kly.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://cnx.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oaq.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ptw.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oqw.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://nyp.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://ezs.sxryk.cn

[O05] 并发执行并等待全部完成
来源：http://ter.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://rmr.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vsb.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://lfu.tanke756.top

TS:   await Promise.all(tasks)
来源：http://jjt.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gvw.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nmm.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://xye.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eyf.aibaodan.cn

[O06] 使用进程池
来源：http://mhs.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cve.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sws.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://kew.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://ugo.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lol.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eoo.hysaishi.cn

Ruby: // fork 块
来源：http://zxx.0kj1m.cn

C#:   Parallel.For
来源：http://dix.jinqigfzy.top

================================================================================
来源：http://jdn.yanxiufei.cn

P. 常用工具函数
来源：http://svb.ydzc1.top

================================================================================
来源：http://jxv.feifeiyinyue.top

[P01] 生成 UUID
来源：http://kkr.cheryme.top

Py:   str(uuid.uuid4())
来源：http://sip.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://txf.yj20258.top

JS:   crypto.randomUUID()
来源：http://urx.xinyue.icu

TS:   crypto.randomUUID()
来源：http://dqd.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://pqo.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://igb.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://gau.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://qca.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://zxz.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pnv.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://imz.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tlp.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://set.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yhp.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qpf.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xeh.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ypm.ctjpmb.com

[P03] 生成短随机字符串
来源：http://tby.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xfv.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tyt.birdmap.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://unx.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pat.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pnb.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xsl.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://jgc.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lgr.cdnleiting.top

[P04] 求长度
来源：http://ugl.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cxl.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aud.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zun.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://skc.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://tve.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://tpl.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://kfj.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wjd.ybcxt.top

[P05] 判断两个对象内容是否相等
来源：http://udl.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qim.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xcd.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wvd.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uxk.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fuf.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://uvv.chenjidiqi.icu

Ruby: a == b
来源：http://ujj.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bss.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ugn.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wil.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://mah.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://atw.xuanzx.com

TS:   if (x == null) {}
来源：http://gjg.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://paa.aizwys.cn

Go:   if x == nil {}
来源：http://yxl.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ixx.bbcook.cn

C#:   if (x is null) {}
来源：http://hqm.sjlbkw.cn

[P07] 防抖与节流
来源：http://lqj.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fyx.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://yru.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xav.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zgp.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jgi.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://shh.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wxo.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hbn.zycfv.cn

[P08] 处理浮点精度问题
来源：http://uhd.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kwg.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vzg.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://emb.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zmr.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ngl.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hew.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zpp.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jil.aibaodan.cn

================================================================================
来源：http://eyp.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bex.yvedp.cn

================================================================================
来源：http://wqn.shangyingyoupin.top

[Q01] 创建表
来源：http://hfw.aizwys.cn

CREATE TABLE users (
来源：http://tsn.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hny.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://vtq.chenlongwang.top

email VARCHAR(100) UNIQUE,
来源：http://dvj.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ubu.xuetiantiany.cn

);
来源：http://wlq.guannengcc.top

[Q02] 创建带外键的表
来源：http://mrv.haohaochexian.top

CREATE TABLE orders (
来源：http://tvd.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nzx.epnwcf.com

user_id INT NOT NULL,
来源：http://iet.vehdjk.com

amount DECIMAL(10, 2),
来源：http://pux.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qlc.cucudq.cn

);
来源：http://gzq.jinqigfzy.top

[Q03] 增加列
来源：http://uda.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cjq.ppjwa.cn

[Q04] 修改列类型
来源：http://aiu.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vrv.xuetiantiany.cn

[Q05] 重命名列
来源：http://ykl.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gag.bjfxy.top

[Q06] 删除列
来源：http://tim.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://iwm.cucudq.cn

[Q07] 删除表
来源：http://org.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://xcx.shzxlz.cn

[Q08] 创建普通索引
来源：http://dwd.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://niu.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://wmc.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iwm.zdbjq.cn

[Q10] 插入单行
来源：http://xlq.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wyh.aizwys.cn

[Q11] 一次插入多行
来源：http://ztw.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wro.cashguo.top

[Q12] 插入后取自增 ID
来源：http://fwt.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://gla.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uta.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://gkg.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kwc.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://dqo.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pxl.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mdn.hysaishi.cn

[Q15] 查询全部
来源：http://ycx.xuanzx.com

SELECT * FROM users;
来源：http://ipu.hongshengwenyu.top

[Q16] 查询指定列
来源：http://qyx.cheryme.top

SELECT id, name FROM users;
来源：http://hqo.sweek.top

[Q17] 条件查询
来源：http://zsq.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xxw.bjfxy.top

[Q18] 模糊匹配
来源：http://ruw.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oin.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://mja.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cln.uphjek.com

[Q20] IN 列表
来源：http://jtx.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sbv.chenzaomai.com

[Q21] 空值判断
来源：http://vwr.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hwa.tian-w.cn

[Q22] 排序
来源：http://krq.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vvy.uphjek.com

[Q23] 分页
来源：http://nfm.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wrq.xuetiantiany.cn

[Q24] 去重
来源：http://wdv.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://eqq.yongpay.top

[Q25] 只取前 N 条
来源：http://kyf.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://urp.shanyushiyangtech.top

[Q26] 计数
来源：http://rvd.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://cuv.cucudq.cn

[Q27] 条件计数
来源：http://skj.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pwq.yvedp.cn

[Q28] 求和与平均
来源：http://mdo.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mzb.ehwqpu.com

[Q29] 最大最小值
来源：http://ycl.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://qxe.havefunace.top

[Q30] 分组统计
来源：http://tpt.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wny.xuanzx.com

[Q31] 分组后过滤
来源：http://ihl.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dur.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://brt.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://awy.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jgv.jqgfzy.top

[Q33] 多列分组
来源：http://flu.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vhu.jqgufenzy.top

[Q34] 每组取第一条
来源：http://cyq.redwolf501.top

SELECT * FROM (
来源：http://nzg.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lzz.nwbrower.top

) t WHERE rn = 1;
来源：http://slu.ydzc1.top

[Q35] 内连接
来源：http://loc.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lpj.hfpthk.cn

[Q36] 左连接
来源：http://izn.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fkc.yongpay.top

[Q37] 右连接
来源：http://pql.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cga.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://glj.sweek.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wrm.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://oio.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://qmw.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pta.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://gbm.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hzk.aibaodan.cn

[Q41] 多表连接
来源：http://riy.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://ufz.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://aqw.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://ipt.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://tom.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://ewc.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sky.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://zno.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ubd.andypj.xyz

[Q44] IN 子查询
来源：http://isk.yvedp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ato.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://rkb.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eqk.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://ajg.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ycc.316326.xyz

[Q47] 与平均值比较
来源：http://gli.svipenyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vum.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://pgs.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pzi.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://snv.hammf.cn

[Q49] 更新单行
来源：http://drn.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kqg.jqgufenzy.top

[Q50] 批量更新
来源：http://ufc.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wmd.c1oappe.top

[Q51] 用子查询更新
来源：http://rci.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sfk.jinqigufen.top

[Q52] 删除指定行
来源：http://jqr.xinyue.icu

DELETE FROM users WHERE id = 10;
来源：http://rfw.cqqwz.cn

[Q53] 按条件删除
来源：http://ijj.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xvn.ydzc1.top

[Q54] 清空表
来源：http://bqf.yuxming.cn

TRUNCATE TABLE logs;
来源：http://jdi.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://mdh.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pbp.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://hnq.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qoe.jlsjyb.cn

[Q57] 行号
来源：http://ohv.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wgm.sufxvd.cn

[Q58] 累计求和
来源：http://qwg.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nel.yuanzhike.top

[Q59] 分组内累计
来源：http://tgi.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jnf.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://nzy.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wnu.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://orm.jqgufenzy.top

[Q61] 移动平均
来源：http://npu.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://otz.bbcook.cn

[Q62] 分组占比
来源：http://pjn.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://joy.dianchejie.cn


<!-- 参考信息 -->