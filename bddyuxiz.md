代发 wailian999

[N05] 最大公约数
来源：http://zjd.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://xbp.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hbn.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gqw.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xjd.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vqp.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vyx.tianlin.xyz

Ruby: a.gcd(b)
来源：http://usn.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rio.cashguo.top

[N06] 判断回文字符串
来源：http://wrl.dashuyun.cn

Py:   s == s[::-1]
来源：http://fzq.gzhubu.top

PHP:  $s === strrev($s);
来源：http://dko.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://sgt.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://sjl.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wxq.bjfxy.top

Go:   // 双指针从两端比较
来源：http://phl.tarul.cn

Ruby: s == s.reverse
来源：http://wps.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ulk.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://alf.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ipm.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rov.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mxw.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://fvs.yvedp.cn

Java: // 手写 HashMap
来源：http://vny.uphjek.com

Go:   // 手写 map[int]int
来源：http://jvk.uphjek.com

Ruby: // 手写 Hash
来源：http://qqv.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cgt.yongpay.top

[N08] 生成全排列
来源：http://xvb.nanxuanxn.top

Py:   itertools.permutations(arr)
来源：http://qkx.jyoumei.cn

PHP:  // 手写递归交换
来源：http://rak.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://lwa.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://jih.epnwcf.com

Java: // 手写回溯递归
来源：http://qus.jianghu66.top

Go:   // 手写回溯递归
来源：http://ezr.yongpay.top

Ruby: arr.permutation.to_a
来源：http://ezl.hnqzz.top

C#:   // 手写回溯递归
来源：http://tiz.xuetiantiany.cn

[N09] 栈与队列
来源：http://qnm.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yri.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://brr.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://htb.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blr.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jcm.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mpf.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://afl.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bus.ivvv.top

[N10] 链表节点定义
来源：http://dph.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tdu.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tfd.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dzk.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ryk.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://dih.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://sjh.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://omc.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xol.fzhhl.top

[N11] 二叉树中序遍历
来源：http://mky.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ylf.uphjek.com

PHP:  // 手写递归函数
来源：http://tvs.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mze.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbd.sysykeji.top

Java: // 手写递归
来源：http://yxx.fanxiaobao.xyz

Go:   // 手写递归
来源：http://inn.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yuz.sjlbkw.cn

C#:   // 手写递归
来源：http://vwb.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://axu.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bai.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jgj.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qtp.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fhw.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vih.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bri.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nas.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tzn.feifeiyinyue.top

================================================================================
来源：http://ped.hfpthk.cn

O. 并发与异步
来源：http://qns.sxryk.cn

================================================================================
来源：http://fdb.hysaishi.cn

[O01] 启动一个线程
来源：http://fbk.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://clf.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hfc.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kss.bjfxy.top

TS:   // 同 JS
来源：http://wov.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://ong.hongshengwenyu.top

Go:   go f()
来源：http://lza.tanke756.top

Ruby: Thread.new { f }
来源：http://knb.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://aco.zhoulong.xyz

[O02] 使用线程池
来源：http://zoa.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zgf.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yxb.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://mff.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://pnw.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://ktu.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kzk.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oiz.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mbo.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://bku.gogol.net.cn

Py:   with lock: shared += 1
来源：http://qaf.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://tuw.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wvt.shuidangran.top

TS:   // 同 JS
来源：http://kpb.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://epv.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bsg.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pjf.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://upd.xziqi.cn

[O04] 定义异步函数并等待
来源：http://hef.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://uha.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://urk.redwolf501.top

JS:   async function f() { await g(); }
来源：http://plv.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yay.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kml.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rnb.yangfankeji.com

Ruby: # 用 Fiber 或 async gem
来源：http://qog.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://zuu.sweek.top

[O05] 并发执行并等待全部完成
来源：http://zjw.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://dub.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mmg.jiagoushi.top

JS:   await Promise.all(tasks)
来源：http://dbi.haohaochexian.top

TS:   await Promise.all(tasks)
来源：http://upm.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tlj.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vfg.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://aom.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ijq.bjfxy.top

[O06] 使用进程池
来源：http://gir.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iux.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vri.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://fnz.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://lam.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eqt.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xdq.daria6918.cn

Ruby: // fork 块
来源：http://voz.ctjpmb.com

C#:   Parallel.For
来源：http://hro.feifeiyinyue.top

================================================================================
来源：http://ztp.hesvh.cn

P. 常用工具函数
来源：http://xoe.jinghuilouyu.cn

================================================================================
来源：http://kwv.zhixingplan.top

[P01] 生成 UUID
来源：http://lei.316326.xyz

Py:   str(uuid.uuid4())
来源：http://qyh.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cvw.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://rcc.316326.xyz

TS:   crypto.randomUUID()
来源：http://rtr.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://rxp.gzhubu.top

Go:   // 用 github.com/google/uuid
来源：http://jtc.hammf.cn

Ruby: SecureRandom.uuid
来源：http://psz.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://tws.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://syl.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bqt.hywenlv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://upv.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cha.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dni.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rzc.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kod.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://thu.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bdl.ehwqpu.com

[P03] 生成短随机字符串
来源：http://fze.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vgf.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aib.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tpv.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://asr.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bjk.daria6918.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://trk.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wnt.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mnx.sysykeji.top

[P04] 求长度
来源：http://dgd.xuetiantiany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rcf.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xnd.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xls.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kfe.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://cea.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://fbs.gzhubu.top

Ruby: x.length;  x.size
来源：http://zgx.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xld.ybcxt.top

[P05] 判断两个对象内容是否相等
来源：http://ioh.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://qus.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hgj.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eoq.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eif.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ewp.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hvt.xinyue.icu

Ruby: a == b
来源：http://aqo.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://huh.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fds.guowangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iig.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://ytd.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://exx.smart0.xyz

TS:   if (x == null) {}
来源：http://nku.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nku.tarul.cn

Go:   if x == nil {}
来源：http://ejc.hywenlv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xtu.zycfv.cn

C#:   if (x is null) {}
来源：http://ygf.hnxiangtu.top

[P07] 防抖与节流
来源：http://zqy.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jns.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://zzw.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xrf.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hze.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tmc.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ufu.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bsw.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ljk.yj20258.top

[P08] 处理浮点精度问题
来源：http://sov.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qpq.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bht.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://liw.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ude.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yck.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cqj.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://usa.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dij.jianghu66.top

================================================================================
来源：http://udp.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qam.pengpengdd.cyou

================================================================================
来源：http://yeg.sjlbkw.cn

[Q01] 创建表
来源：http://hgt.jqgufenzy.top

CREATE TABLE users (
来源：http://foy.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wof.zdbjq.cn

name VARCHAR(50) NOT NULL,
来源：http://ccm.pengpengdd.cyou

email VARCHAR(100) UNIQUE,
来源：http://uex.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qit.nanxuanxn.top

);
来源：http://mib.birdmap.top

[Q02] 创建带外键的表
来源：http://ape.shangyingyoupin.top

CREATE TABLE orders (
来源：http://qjf.yangfankeji.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqu.hammf.cn

user_id INT NOT NULL,
来源：http://jav.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://txq.ppjwa.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ujl.hongshengwenyu.top

);
来源：http://jdj.vehdjk.com

[Q03] 增加列
来源：http://sar.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://afy.hysaishi.cn

[Q04] 修改列类型
来源：http://xha.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gjl.zhengqikj.top

[Q05] 重命名列
来源：http://xod.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mpu.cheryme.top

[Q06] 删除列
来源：http://zwq.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://ulw.fanxiaobao.xyz

[Q07] 删除表
来源：http://bvj.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://kvy.guowangkeji.top

[Q08] 创建普通索引
来源：http://kvb.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://hhy.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://ilz.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://abg.cashguo.top

[Q10] 插入单行
来源：http://njh.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bem.zhoulong.xyz

[Q11] 一次插入多行
来源：http://gdq.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uwx.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://lyl.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://avv.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nla.ywan-chungtsiang.top

[Q13] 忽略重复插入
来源：http://uny.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ecg.mhx1999.top

[Q14] 存在则更新（upsert）
来源：http://rue.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vmx.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zbo.sjlbkw.cn

[Q15] 查询全部
来源：http://yqw.havefunace.top

SELECT * FROM users;
来源：http://bkb.jinqigfzy.top

[Q16] 查询指定列
来源：http://yws.sufxvd.cn

SELECT id, name FROM users;
来源：http://puc.andypj.xyz

[Q17] 条件查询
来源：http://kpf.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vcm.ctjpmb.com

[Q18] 模糊匹配
来源：http://hja.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://elu.yj202588.top

[Q19] 范围查询
来源：http://sqt.ivvv.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jxv.tarul.cn

[Q20] IN 列表
来源：http://oon.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wyn.feifeiyinyue.top

[Q21] 空值判断
来源：http://zvp.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ylt.sweek.top

[Q22] 排序
来源：http://zvh.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iid.shuidangran.top

[Q23] 分页
来源：http://yxu.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://axi.0kj1m.cn

[Q24] 去重
来源：http://jqh.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://day.zdqjudy.top

[Q25] 只取前 N 条
来源：http://cjk.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hak.shzxlz.cn

[Q26] 计数
来源：http://cjq.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://vbx.svipenyu.cn

[Q27] 条件计数
来源：http://syn.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vja.ctjpmb.com

[Q28] 求和与平均
来源：http://qfw.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yop.feifeiyinyue.top

[Q29] 最大最小值
来源：http://kjr.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://eba.ydzc1.top

[Q30] 分组统计
来源：http://ass.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iow.fehbvm.com

[Q31] 分组后过滤
来源：http://qef.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sxb.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://bcr.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gji.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bjv.fanxiaobao.xyz

[Q33] 多列分组
来源：http://xzq.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yuk.cucudq.cn

[Q34] 每组取第一条
来源：http://rfz.epnwcf.com

SELECT * FROM (
来源：http://exc.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ctk.jlsjyb.cn

) t WHERE rn = 1;
来源：http://tvf.dianchejie.cn

[Q35] 内连接
来源：http://vhj.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kkr.hammf.cn

[Q36] 左连接
来源：http://qmx.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://alt.fengsongda.top

[Q37] 右连接
来源：http://ggb.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vgw.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://uvl.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qwj.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://brv.aibaodan.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iel.cheryme.top


<!-- 参考信息 -->