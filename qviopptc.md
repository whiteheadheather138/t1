代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dci.aizwys.cn

[N06] 判断回文字符串
来源：http://xhp.yuanzhike.top

Py:   s == s[::-1]
来源：http://cam.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://zcz.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://wxa.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://pxr.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mkf.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://fvy.tanke756.top

Ruby: s == s.reverse
来源：http://wtd.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rrt.cashguo.top

[N07] 两数之和（返回下标）
来源：http://pjd.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://arf.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ptw.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wjo.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://jsj.shzxlz.cn

Java: // 手写 HashMap
来源：http://icr.daxiang520.top

Go:   // 手写 map[int]int
来源：http://qlw.jyoumei.cn

Ruby: // 手写 Hash
来源：http://imq.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oqf.ehwqpu.com

[N08] 生成全排列
来源：http://uzd.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://duq.redwolf501.top

PHP:  // 手写递归交换
来源：http://aaa.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://hsw.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://pdv.daxiang520.top

Java: // 手写回溯递归
来源：http://flh.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://qpv.yj20258.top

Ruby: arr.permutation.to_a
来源：http://hht.chenlongwang.top

C#:   // 手写回溯递归
来源：http://qax.aizwys.cn

[N09] 栈与队列
来源：http://mbw.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bru.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://izj.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://czn.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ish.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cft.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qby.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fjj.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pcs.zhiwuduotai.top

[N10] 链表节点定义
来源：http://oei.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zpv.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uwe.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gzz.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cui.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://mrb.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://pwg.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vfl.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rsr.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://sfm.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ydj.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://bea.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aoe.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cny.bbcook.cn

Java: // 手写递归
来源：http://lmh.yanxiufei.cn

Go:   // 手写递归
来源：http://syh.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lwj.cheryme.top

C#:   // 手写递归
来源：http://bbk.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uus.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jbe.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://reg.ehwqpu.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zru.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nkv.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qjp.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uwe.tarul.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jaj.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fai.zhijiandao.cn

================================================================================
来源：http://pup.fengsongda.top

O. 并发与异步
来源：http://jho.yj20258.top

================================================================================
来源：http://qao.snrcjt.cn

[O01] 启动一个线程
来源：http://cmn.hongshengwenyu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://erg.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ymq.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xrm.52xcode.cn

TS:   // 同 JS
来源：http://qju.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://iag.nwbrower.top

Go:   go f()
来源：http://zwp.bbcook.cn

Ruby: Thread.new { f }
来源：http://ydx.yj20258888.top

C#:   Task.Run(() => F());
来源：http://fxz.sysykeji.top

[O02] 使用线程池
来源：http://hyr.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zmy.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mux.cashguo.top

JS:   // worker_threads 线程池
来源：http://cdc.yfazqb.com

TS:   // worker_threads 线程池
来源：http://zmy.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://viy.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cjp.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wge.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cxf.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://uyq.jqgfzy.top

Py:   with lock: shared += 1
来源：http://clt.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://ilc.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qad.jlsjyb.cn

TS:   // 同 JS
来源：http://ctt.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://eyb.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bwd.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ifo.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://iok.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://zoj.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://bbp.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dsn.jianghu66.top

JS:   async function f() { await g(); }
来源：http://pwp.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eed.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ycn.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ycm.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://enr.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://wbj.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://bnf.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://jrg.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ltz.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://rwv.yonumen.top

TS:   await Promise.all(tasks)
来源：http://xgi.ctjpmb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tdf.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xph.birdmap.top

Ruby: threads.map(&:join)
来源：http://vky.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aoh.yuxming.cn

[O06] 使用进程池
来源：http://bvx.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cde.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tmi.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://dlz.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://ylt.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://egq.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://clo.pengpengdd.cyou

Ruby: // fork 块
来源：http://bdd.nanxinkj.top

C#:   Parallel.For
来源：http://exa.shangyingyoupin.top

================================================================================
来源：http://wan.cdnleiting.top

P. 常用工具函数
来源：http://zdb.yangfankeji.com

================================================================================
来源：http://gwr.ctjpmb.com

[P01] 生成 UUID
来源：http://zpr.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://jph.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mgx.tian-w.cn

JS:   crypto.randomUUID()
来源：http://yfg.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://bng.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://ymx.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://ebr.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://poi.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://tcc.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://vjg.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qxq.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://fnh.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xtc.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dri.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nkd.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pbv.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aag.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rqh.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://snj.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fra.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vgu.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ivt.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://flg.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fdp.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xcs.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qxh.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xdj.gogol.net.cn

[P04] 求长度
来源：http://rpb.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qqp.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kld.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iin.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eao.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://znx.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://ism.hfpthk.cn

Ruby: x.length;  x.size
来源：http://ebd.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://lmr.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://fbz.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bhf.hnqzz.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pjf.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fmq.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eqo.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qbz.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ejy.yongpay.top

Ruby: a == b
来源：http://ghe.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xdo.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vyr.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uwd.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://ssf.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pek.dashuyun.cn

TS:   if (x == null) {}
来源：http://brn.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mdb.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://wgv.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rdc.sweek.top

C#:   if (x is null) {}
来源：http://hmq.hongshengwenyu.top

[P07] 防抖与节流
来源：http://lcv.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kho.yj20258.top

PHP:  // 手写时间戳比较
来源：http://dzt.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qkn.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tce.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dmw.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kca.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nnr.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jxp.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://ose.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dcw.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pbh.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ety.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aci.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://liv.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dgu.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vqr.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kce.shzxlz.cn

================================================================================
来源：http://qgx.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ouj.zhijiandao.cn

================================================================================
来源：http://oml.dashuyun.cn

[Q01] 创建表
来源：http://shi.jinqigfzy.top

CREATE TABLE users (
来源：http://lwi.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hmo.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://qzs.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://ume.nwbrower.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oga.yanxiufei.cn

);
来源：http://yev.ctjpmb.com

[Q02] 创建带外键的表
来源：http://shg.gaohongyu789.top

CREATE TABLE orders (
来源：http://vkw.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://boy.yangfankeji.com

user_id INT NOT NULL,
来源：http://hef.ydzc1.top

amount DECIMAL(10, 2),
来源：http://xaz.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zpk.yonumen.top

);
来源：http://bmc.bbcook.cn

[Q03] 增加列
来源：http://pea.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ixr.nanxuanxn.top

[Q04] 修改列类型
来源：http://zby.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://njo.chenlongwang.top

[Q05] 重命名列
来源：http://yrr.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://chs.chenjidiqi.icu

[Q06] 删除列
来源：http://qpj.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://mbh.kuanghao11.cn

[Q07] 删除表
来源：http://dxz.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://vot.tarul.cn

[Q08] 创建普通索引
来源：http://uth.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sfs.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://cvb.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kwk.ybcxt.top

[Q10] 插入单行
来源：http://qrz.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vou.sweek.top

[Q11] 一次插入多行
来源：http://zcv.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cxa.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://rhv.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://lom.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dfm.mhx1999.top

[Q13] 忽略重复插入
来源：http://hzo.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bku.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://tdp.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eii.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://olx.cheryme.top

[Q15] 查询全部
来源：http://vyd.hcnkem.com

SELECT * FROM users;
来源：http://waq.fktsv.cn

[Q16] 查询指定列
来源：http://cec.fzhhl.top

SELECT id, name FROM users;
来源：http://ysu.chenzaomai.com

[Q17] 条件查询
来源：http://eax.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wjz.sweek.top

[Q18] 模糊匹配
来源：http://uki.guannengcc.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ksu.wangdashe.top

[Q19] 范围查询
来源：http://gle.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pfv.jyoumei.cn

[Q20] IN 列表
来源：http://oyg.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cuz.fktsv.cn

[Q21] 空值判断
来源：http://emu.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://sxh.bbcook.cn

[Q22] 排序
来源：http://pwa.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eqb.dashuyun.cn

[Q23] 分页
来源：http://cvo.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yvv.vehdjk.com

[Q24] 去重
来源：http://qkc.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://ltv.cdnleiting.top

[Q25] 只取前 N 条
来源：http://bee.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://swi.aibaodan.cn

[Q26] 计数
来源：http://bxo.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://lha.sufxvd.cn

[Q27] 条件计数
来源：http://azp.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vwu.feifeiyinyue.top

[Q28] 求和与平均
来源：http://wvl.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mxm.fehbvm.com

[Q29] 最大最小值
来源：http://ggk.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://dfu.smart0.xyz

[Q30] 分组统计
来源：http://nor.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xyc.ppjwa.cn

[Q31] 分组后过滤
来源：http://biu.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qcw.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://lip.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ixr.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://afa.guowangkeji.top

[Q33] 多列分组
来源：http://dpu.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lln.jqgufenzy.top

[Q34] 每组取第一条
来源：http://chc.ctjpmb.com

SELECT * FROM (
来源：http://ktl.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ysk.zycfv.cn

) t WHERE rn = 1;
来源：http://dst.nanxinkj.top

[Q35] 内连接
来源：http://wtg.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qvd.pycfn.com

[Q36] 左连接
来源：http://tqx.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://deg.bbcook.cn

[Q37] 右连接
来源：http://emv.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://opz.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ruv.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ets.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://oko.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://cln.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://moa.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://urm.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jos.fzhhl.top

[Q41] 多表连接
来源：http://ikz.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://wvn.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://hix.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://dbg.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://fgs.zhoulong.xyz


<!-- 参考信息 -->