代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pcc.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oor.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sew.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ocy.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zzl.zdqjudy.top

[N10] 链表节点定义
来源：http://ctb.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ytm.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rcm.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://chp.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cye.birdmap.top

Java: class Node { int v; Node next; }
来源：http://eun.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://evc.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://asj.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://dgg.ybcxt.top

[N11] 二叉树中序遍历
来源：http://ait.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kor.meibo888.top

PHP:  // 手写递归函数
来源：http://tby.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bnt.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oqr.jyoumei.cn

Java: // 手写递归
来源：http://ftt.tarul.cn

Go:   // 手写递归
来源：http://amz.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://stb.cheryme.top

C#:   // 手写递归
来源：http://rtr.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hob.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iya.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ooj.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ogq.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://agw.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://axw.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pko.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://csj.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cvl.hcnkem.com

================================================================================
来源：http://mxx.xingfuxueyuan.xyz

O. 并发与异步
来源：http://ass.yj202588.top

================================================================================
来源：http://qfb.yongpay.top

[O01] 启动一个线程
来源：http://tzq.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kso.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tij.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mwr.pengpengdd.cyou

TS:   // 同 JS
来源：http://jkq.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://tuz.fengsongda.top

Go:   go f()
来源：http://oxs.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://yqy.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://lmy.dianchejie.cn

[O02] 使用线程池
来源：http://ztq.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fja.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zzf.wangdashe.top

JS:   // worker_threads 线程池
来源：http://blp.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://fid.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ttm.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pru.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dig.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oiq.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://mex.hnqzz.top

Py:   with lock: shared += 1
来源：http://gvw.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://unz.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://crx.redwolf501.top

TS:   // 同 JS
来源：http://syz.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://rde.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ozq.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fpa.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://lrt.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://nsj.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://qfi.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jpu.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://rrp.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uho.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xws.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mxz.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://npk.birdmap.top

C#:   async Task F() { await G(); }
来源：http://cmq.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://iry.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://jhg.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rle.tarul.cn

JS:   await Promise.all(tasks)
来源：http://iph.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://dae.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ggd.cashguo.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yni.redwolf501.top

Ruby: threads.map(&:join)
来源：http://akh.jiagoushi.top

C#:   await Task.WhenAll(t1, t2)
来源：http://spg.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://qgl.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zpb.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rtp.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://uss.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://wny.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://atz.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gyi.xuetiantiany.cn

Ruby: // fork 块
来源：http://gss.zhoulong.xyz

C#:   Parallel.For
来源：http://cos.zdqjudy.top

================================================================================
来源：http://cyq.zhijiandao.cn

P. 常用工具函数
来源：http://yoq.sjlbkw.cn

================================================================================
来源：http://pfa.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://pcj.cqqwz.cn

Py:   str(uuid.uuid4())
来源：http://arh.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ixu.ybcxt.top

JS:   crypto.randomUUID()
来源：http://plm.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://vxq.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://the.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://qvt.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://dgq.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://kha.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://jtf.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qvw.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://wqj.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ngi.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xkd.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pmd.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aan.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hoz.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ggc.c1oappe.top

[P03] 生成短随机字符串
来源：http://hto.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vfc.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fnm.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qrj.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://euz.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lbf.9152youxi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ryj.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://svl.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://unn.zhiwuduotai.top

[P04] 求长度
来源：http://ljz.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ehq.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ynm.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzj.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dog.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://tpp.hammf.cn

Go:   len(arr);  len(m)
来源：http://bcn.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://akr.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://gyo.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://qob.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://slf.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rgw.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yxd.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xfk.zycfv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lqu.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lhy.zhijiandao.cn

Ruby: a == b
来源：http://era.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rfa.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fje.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://upf.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://dfg.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lxj.shuidangran.top

TS:   if (x == null) {}
来源：http://tbf.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fgx.cheryme.top

Go:   if x == nil {}
来源：http://bmu.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jdq.ppjwa.cn

C#:   if (x is null) {}
来源：http://gim.sjlbkw.cn

[P07] 防抖与节流
来源：http://qua.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lkk.hammf.cn

PHP:  // 手写时间戳比较
来源：http://zvs.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://viw.svipenyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxn.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yzt.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ijt.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://qrf.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sik.hcnkem.com

[P08] 处理浮点精度问题
来源：http://xvk.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fti.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tem.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ika.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ndr.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aki.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bbj.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gul.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oql.feifeiyinyue.top

================================================================================
来源：http://tef.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rbp.fehbvm.com

================================================================================
来源：http://qxn.shanyushiyangkeji.top

[Q01] 创建表
来源：http://irs.hywenlv.cn

CREATE TABLE users (
来源：http://yra.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ohu.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://ujg.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://thz.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aaa.jqgfzy.top

);
来源：http://tjt.yvedp.cn

[Q02] 创建带外键的表
来源：http://nig.pengpengdd.cyou

CREATE TABLE orders (
来源：http://ygy.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://agb.zhixingplan.top

user_id INT NOT NULL,
来源：http://syt.cucudq.cn

amount DECIMAL(10, 2),
来源：http://svm.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xnp.daxiang520.top

);
来源：http://ity.jqgufenzy.top

[Q03] 增加列
来源：http://ydn.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cfa.xziqi.cn

[Q04] 修改列类型
来源：http://usz.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lca.hysaishi.cn

[Q05] 重命名列
来源：http://wmo.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cwg.pengpengdd.cyou

[Q06] 删除列
来源：http://mmc.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://zsf.shangyingyoupin.top

[Q07] 删除表
来源：http://msr.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://wbj.pengpengdd.cyou

[Q08] 创建普通索引
来源：http://bqo.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://bei.chenzaomai.com

[Q09] 创建唯一索引
来源：http://gia.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ult.yfazqb.com

[Q10] 插入单行
来源：http://odh.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ckn.mhx1999.top

[Q11] 一次插入多行
来源：http://fzo.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bfu.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://qkq.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://fgh.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cyd.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://jgq.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rge.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://rjm.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hza.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://khr.ehwqpu.com

[Q15] 查询全部
来源：http://ygn.ybcxt.top

SELECT * FROM users;
来源：http://vbe.hysaishi.cn

[Q16] 查询指定列
来源：http://oae.smart0.xyz

SELECT id, name FROM users;
来源：http://gco.tarul.cn

[Q17] 条件查询
来源：http://ogh.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zhj.gzhubu.top

[Q18] 模糊匹配
来源：http://pdw.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fah.shanyushiyangtech.top

[Q19] 范围查询
来源：http://bvm.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yrv.tian-w.cn

[Q20] IN 列表
来源：http://xhe.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cjo.yuanzhike.top

[Q21] 空值判断
来源：http://ykh.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iqh.xylfe.cn

[Q22] 排序
来源：http://nro.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mpv.jinqigfzy.top

[Q23] 分页
来源：http://bcl.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://caz.316326.xyz

[Q24] 去重
来源：http://kzl.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://het.sufxvd.cn

[Q25] 只取前 N 条
来源：http://xja.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hom.dashuyun.cn

[Q26] 计数
来源：http://lrh.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://sga.fehbvm.com

[Q27] 条件计数
来源：http://qlx.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ler.zhongyouzk.top

[Q28] 求和与平均
来源：http://xup.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rbx.redwolf501.top

[Q29] 最大最小值
来源：http://wea.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yrm.jinghuilouyu.cn

[Q30] 分组统计
来源：http://dez.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://one.tianlin.xyz

[Q31] 分组后过滤
来源：http://osy.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ptz.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://lki.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rwl.yonumen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ezd.bjfxy.top

[Q33] 多列分组
来源：http://bzp.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rkg.tarul.cn

[Q34] 每组取第一条
来源：http://cld.chenzaomai.com

SELECT * FROM (
来源：http://rwb.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://njh.hnqzz.top

) t WHERE rn = 1;
来源：http://hfj.fehbvm.com

[Q35] 内连接
来源：http://xbx.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yql.aizwys.cn

[Q36] 左连接
来源：http://wjl.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://piv.c1oappe.top

[Q37] 右连接
来源：http://zir.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ymh.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://lik.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rfb.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://gtj.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://plk.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fln.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ghm.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tww.daria6918.cn

[Q41] 多表连接
来源：http://mve.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pti.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://nhp.gogol.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://qyq.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://yaf.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://erz.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bbr.jqgufenzy.top

[Q43] 标量子查询
来源：http://tfe.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mtn.shangyingyoupin.top

[Q44] IN 子查询
来源：http://pcq.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zcs.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://idy.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tup.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hxn.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yio.0kj1m.cn

[Q47] 与平均值比较
来源：http://pww.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sll.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://gtk.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rgy.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://ahc.aizwys.cn

[Q49] 更新单行
来源：http://gcc.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jzu.smart0.xyz

[Q50] 批量更新
来源：http://koi.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rui.pycfn.com

[Q51] 用子查询更新
来源：http://jav.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ygr.gzhubu.top

[Q52] 删除指定行
来源：http://wac.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://dzd.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://mdf.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nta.hfpthk.cn

[Q54] 清空表
来源：http://rvs.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://deg.xuanzx.com

[Q55] 排名（并列占位）
来源：http://pic.jinqigufen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mvq.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://ujl.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ubp.hnqzz.top

[Q57] 行号
来源：http://daz.ydzc1.top


<!-- 参考信息 -->