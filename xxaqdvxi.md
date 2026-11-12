代发 wailian999

[N09] 栈与队列
来源：http://wdy.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ixb.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ipa.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tvi.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lwj.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jda.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nwg.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zth.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ala.daria6918.cn

[N10] 链表节点定义
来源：http://uqu.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yxj.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xvx.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ulj.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oxx.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://yxr.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://ljv.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ddn.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pyp.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://veb.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qan.ppjwa.cn

PHP:  // 手写递归函数
来源：http://hrq.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cya.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://szb.snrcjt.cn

Java: // 手写递归
来源：http://qoj.chenjidiqi.icu

Go:   // 手写递归
来源：http://nci.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gvt.nwbrower.top

C#:   // 手写递归
来源：http://xxv.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://adt.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ymw.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rhj.52xcode.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rpj.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lzf.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kyl.yj202588.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qvf.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kej.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mvh.gotoacloud.top

================================================================================
来源：http://bpq.ivvv.top

O. 并发与异步
来源：http://tuy.tian-w.cn

================================================================================
来源：http://hem.yj202588.top

[O01] 启动一个线程
来源：http://xfx.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yxi.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pca.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gub.c1oappe.top

TS:   // 同 JS
来源：http://fxs.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://pbq.9152youxi.cn

Go:   go f()
来源：http://xfa.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://ylo.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://nny.yueranfly.top

[O02] 使用线程池
来源：http://sxc.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cza.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://atb.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://xmg.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://qkx.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://axa.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bdt.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tjb.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zgz.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://fqx.epnwcf.com

Py:   with lock: shared += 1
来源：http://snz.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://weg.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pgt.nwbrower.top

TS:   // 同 JS
来源：http://qkb.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://oca.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://alk.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tpw.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://ltr.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://zox.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://ccm.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ojx.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://ivu.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wov.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kal.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://brz.vqdsnc.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jwb.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://imr.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://meh.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://lwf.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xne.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://imq.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://ify.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://djt.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yde.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://oyh.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ozi.aibaodan.cn

[O06] 使用进程池
来源：http://wpv.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ywy.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://afk.yongpay.top

JS:   // child_process / cluster 模块
来源：http://jek.0kj1m.cn

TS:   // child_process / cluster 模块
来源：http://ytw.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qtf.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mvh.wangshuangyany.cn

Ruby: // fork 块
来源：http://gmq.shanyushiyangtech.top

C#:   Parallel.For
来源：http://bhk.nanxinkj.top

================================================================================
来源：http://lsq.chenjidiqi.icu

P. 常用工具函数
来源：http://xkj.shzxlz.cn

================================================================================
来源：http://szy.yvedp.cn

[P01] 生成 UUID
来源：http://ysd.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://kzj.meibo888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rcp.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://cmg.yj202588.top

TS:   crypto.randomUUID()
来源：http://esf.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://isu.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://uen.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://gjq.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://wwg.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://rlq.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bjj.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ykg.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kgx.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://edo.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vqg.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lbc.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uvf.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uhk.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://icc.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://thw.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dzm.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ehc.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cig.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tje.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kii.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ivz.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rsb.andypj.xyz

[P04] 求长度
来源：http://nvv.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://izb.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://omp.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wdo.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zze.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://caw.uphjek.com

Go:   len(arr);  len(m)
来源：http://hjr.tian-w.cn

Ruby: x.length;  x.size
来源：http://ffb.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://khp.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://whi.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yzv.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kim.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://clx.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ikh.hfpthk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fdb.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://yas.wangshuangyany.cn

Ruby: a == b
来源：http://ebt.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ycw.fktsv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rzg.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iko.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://hhd.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vrl.fehbvm.com

TS:   if (x == null) {}
来源：http://jxw.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dhz.jinqigufen.top

Go:   if x == nil {}
来源：http://udu.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yem.dianchejie.cn

C#:   if (x is null) {}
来源：http://hky.pycfn.com

[P07] 防抖与节流
来源：http://kgp.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yqu.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://cqq.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ale.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nao.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pkp.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wxz.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://syi.pengpengdd.cyou

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pbe.pengpengdd.cyou

[P08] 处理浮点精度问题
来源：http://flr.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ozo.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tuw.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bhx.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hzt.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://trq.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cjc.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mav.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kuy.fehbvm.com

================================================================================
来源：http://bpa.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pwi.c1oappe.top

================================================================================
来源：http://ifl.hysaishi.cn

[Q01] 创建表
来源：http://uns.uphjek.com

CREATE TABLE users (
来源：http://osj.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dhu.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://sea.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://ovx.wangdashe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xwr.chenjidiqi.icu

);
来源：http://kws.shuidangran.top

[Q02] 创建带外键的表
来源：http://nhb.hysaishi.cn

CREATE TABLE orders (
来源：http://sps.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wlo.ydzc1.top

user_id INT NOT NULL,
来源：http://isa.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://lqj.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://scc.chenlongwang.top

);
来源：http://ucf.ctjpmb.com

[Q03] 增加列
来源：http://ylr.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xla.jinqigufen.top

[Q04] 修改列类型
来源：http://moj.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fmm.smart0.xyz

[Q05] 重命名列
来源：http://hfy.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mpl.nwbrower.top

[Q06] 删除列
来源：http://fjt.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yfk.zhengqikj.top

[Q07] 删除表
来源：http://csu.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://xwj.9152youxi.cn

[Q08] 创建普通索引
来源：http://kyg.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wpc.hywenlv.cn

[Q09] 创建唯一索引
来源：http://zxn.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dyc.yuanzhike.top

[Q10] 插入单行
来源：http://ggs.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ief.birdmap.top

[Q11] 一次插入多行
来源：http://cbe.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://svp.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://mgl.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ejl.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ovb.hysaishi.cn

[Q13] 忽略重复插入
来源：http://djy.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tnt.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://lvz.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dhs.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gtr.zycfv.cn

[Q15] 查询全部
来源：http://hlu.jqgfzy.top

SELECT * FROM users;
来源：http://bee.fehbvm.com

[Q16] 查询指定列
来源：http://bsv.haohaochexian.top

SELECT id, name FROM users;
来源：http://myp.sufxvd.cn

[Q17] 条件查询
来源：http://rku.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cee.yongpay.top

[Q18] 模糊匹配
来源：http://crz.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pqv.gzhubu.top

[Q19] 范围查询
来源：http://xsv.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ugv.cashguo.top

[Q20] IN 列表
来源：http://ref.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wmh.meibo888.top

[Q21] 空值判断
来源：http://gsw.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aoc.smart0.xyz

[Q22] 排序
来源：http://llv.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lbj.gaohongyu789.top

[Q23] 分页
来源：http://tpn.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pgc.zhongyouzk.top

[Q24] 去重
来源：http://ren.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://eng.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://ura.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://avh.hnxiangtu.top

[Q26] 计数
来源：http://dqa.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://ejy.nwbrower.top

[Q27] 条件计数
来源：http://tof.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vsw.jlsjyb.cn

[Q28] 求和与平均
来源：http://uwd.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qxg.sweek.top

[Q29] 最大最小值
来源：http://ykb.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gko.yj20258.top

[Q30] 分组统计
来源：http://zfn.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ice.yfazqb.com

[Q31] 分组后过滤
来源：http://jvr.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mxx.wangdashe.top

[Q32] 分组拼接字符串
来源：http://hsw.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bkz.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uio.zhiwuduotai.top

[Q33] 多列分组
来源：http://iab.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uuu.xuanzx.com

[Q34] 每组取第一条
来源：http://gvu.snrcjt.cn

SELECT * FROM (
来源：http://dcs.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iym.hcnkem.com

) t WHERE rn = 1;
来源：http://wxd.xuanzx.com

[Q35] 内连接
来源：http://gmt.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vwb.shangyingyoupin.top

[Q36] 左连接
来源：http://lzg.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cjh.yonumen.top

[Q37] 右连接
来源：http://ubi.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wts.ydzc1.top

[Q38] 全外连接（PostgreSQL）
来源：http://ryy.dashuyun.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ael.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://wba.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dvu.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://men.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://wuy.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oky.zhixingplan.top

[Q41] 多表连接
来源：http://ter.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vbj.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://cwk.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://scd.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://ctr.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://wcc.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://chw.zdbjq.cn

[Q43] 标量子查询
来源：http://xuy.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oml.pengpengdd.cyou

[Q44] IN 子查询
来源：http://mto.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ztu.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://kvi.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://apr.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mzq.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpk.meibo888.top

[Q47] 与平均值比较
来源：http://mda.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tgq.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://isn.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vtv.ywan-chungtsiang.top

SELECT * FROM t WHERE c > 5;
来源：http://vou.52xcode.cn

[Q49] 更新单行
来源：http://ggn.jiagoushi.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ycb.jqgufenzy.top

[Q50] 批量更新
来源：http://ogf.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://usr.ydjk.org.cn

[Q51] 用子查询更新
来源：http://nai.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pyl.zhongyouzk.top

[Q52] 删除指定行
来源：http://sqw.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://eok.hcnkem.com

[Q53] 按条件删除
来源：http://xkm.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sxy.jinqigfzy.top

[Q54] 清空表
来源：http://psu.nwbrower.top

TRUNCATE TABLE logs;
来源：http://fip.mhx1999.top

[Q55] 排名（并列占位）
来源：http://cqi.zdbjq.cn


<!-- 参考信息 -->