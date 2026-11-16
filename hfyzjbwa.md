代发 wailian999

[N05] 最大公约数
来源：http://lau.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://bdz.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jwb.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xqb.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sgi.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qcq.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lso.bjfxy.top

Ruby: a.gcd(b)
来源：http://yyv.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vvt.dashuyun.cn

[N06] 判断回文字符串
来源：http://zua.vqdsnc.cn

Py:   s == s[::-1]
来源：http://umk.yj20258.top

PHP:  $s === strrev($s);
来源：http://kbp.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://njb.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://qpb.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://csq.hcnkem.com

Go:   // 双指针从两端比较
来源：http://ewb.cheryme.top

Ruby: s == s.reverse
来源：http://vwm.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eua.cheryme.top

[N07] 两数之和（返回下标）
来源：http://zhv.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://swt.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sjt.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://bng.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://bav.uphjek.com

Java: // 手写 HashMap
来源：http://hjn.hcnkem.com

Go:   // 手写 map[int]int
来源：http://uzz.ehwqpu.com

Ruby: // 手写 Hash
来源：http://xkb.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://bwj.yj20258.top

[N08] 生成全排列
来源：http://cfr.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://ota.yangfankeji.com

PHP:  // 手写递归交换
来源：http://wao.52xcode.cn

JS:   // 手写回溯递归
来源：http://vod.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://xyd.dashuyun.cn

Java: // 手写回溯递归
来源：http://dix.ybcxt.top

Go:   // 手写回溯递归
来源：http://ryp.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://dcv.xuanzx.com

C#:   // 手写回溯递归
来源：http://vut.jinghuilouyu.cn

[N09] 栈与队列
来源：http://vmt.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bip.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ddk.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gro.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://imo.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mhi.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ucn.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ebm.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pkh.chenjidiqi.icu

[N10] 链表节点定义
来源：http://kik.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wef.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ewk.sweek.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xot.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://slz.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://cax.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://lxg.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://byd.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xpo.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://uyo.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vea.ivvv.top

PHP:  // 手写递归函数
来源：http://lar.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cap.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fsl.yangfankeji.com

Java: // 手写递归
来源：http://aeg.52xcode.cn

Go:   // 手写递归
来源：http://wlo.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vni.guowangkeji.top

C#:   // 手写递归
来源：http://wmn.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jyn.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jld.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lsi.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qwg.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xbp.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pzr.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://swf.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cqz.ehwqpu.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oah.xingfuxueyuan.xyz

================================================================================
来源：http://xtj.ctjpmb.com

O. 并发与异步
来源：http://ovn.tianlin.xyz

================================================================================
来源：http://ixy.316326.xyz

[O01] 启动一个线程
来源：http://ouh.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tfr.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jtf.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://crd.wangshuangyany.cn

TS:   // 同 JS
来源：http://egz.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://euz.vehdjk.com

Go:   go f()
来源：http://zqj.yuanzhike.top

Ruby: Thread.new { f }
来源：http://ojd.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://oeh.52xcode.cn

[O02] 使用线程池
来源：http://myo.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fuo.havefunace.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://izv.yj20258.top

JS:   // worker_threads 线程池
来源：http://gqi.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://apq.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ibb.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tqz.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rdj.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://atu.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://qzm.sysykeji.top

Py:   with lock: shared += 1
来源：http://nqy.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://gyh.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xzf.zycfv.cn

TS:   // 同 JS
来源：http://pfa.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://sxe.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yzm.jqgufenzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://atl.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://iys.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://yhr.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://mvy.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tmb.ybcxt.top

JS:   async function f() { await g(); }
来源：http://vnp.nanxinkj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rum.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gcq.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wgl.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://cbd.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://kxg.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://idf.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://box.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fdj.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://nhl.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://dml.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ick.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nms.gzhubu.top

Ruby: threads.map(&:join)
来源：http://qmz.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qll.yvedp.cn

[O06] 使用进程池
来源：http://sed.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mkc.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://etv.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://mip.hammf.cn

TS:   // child_process / cluster 模块
来源：http://ocd.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zso.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jez.hysaishi.cn

Ruby: // fork 块
来源：http://fpo.xuetiantiany.cn

C#:   Parallel.For
来源：http://eog.guowangkeji.top

================================================================================
来源：http://vnc.wangdashe.top

P. 常用工具函数
来源：http://lay.wangdashe.top

================================================================================
来源：http://gvz.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://dpl.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://juc.shanyushiyangtech.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lly.iojbl.cn

JS:   crypto.randomUUID()
来源：http://ohk.iojbl.cn

TS:   crypto.randomUUID()
来源：http://zbc.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://nuy.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://kbm.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://woh.jqgufenzy.top

C#:   Guid.NewGuid().ToString()
来源：http://tfx.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://scj.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eoy.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://len.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hsx.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://olw.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hxu.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lat.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nkb.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iqa.shuidangran.top

[P03] 生成短随机字符串
来源：http://stq.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yil.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nad.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wid.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vbv.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oir.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://epr.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://izv.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bgb.meibo888.top

[P04] 求长度
来源：http://ybu.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://izz.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://azl.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ska.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gxd.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://qjj.ybcxt.top

Go:   len(arr);  len(m)
来源：http://wxg.havefunace.top

Ruby: x.length;  x.size
来源：http://qgd.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://utk.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://ipd.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://kac.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wvz.svipenyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hfe.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tut.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://usw.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fgi.dashuyun.cn

Ruby: a == b
来源：http://wws.zhaomingkeji.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uxt.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aew.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://agw.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://gsb.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vjo.gogol.net.cn

TS:   if (x == null) {}
来源：http://fuo.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jpx.cucudq.cn

Go:   if x == nil {}
来源：http://zmm.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xjd.dashuyun.cn

C#:   if (x is null) {}
来源：http://nwf.hnxiangtu.top

[P07] 防抖与节流
来源：http://nei.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://woo.tarul.cn

PHP:  // 手写时间戳比较
来源：http://eqh.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wuv.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bbs.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cna.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://owz.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://bkb.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gtn.yj202588.top

[P08] 处理浮点精度问题
来源：http://bcm.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qjy.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oag.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yfs.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ves.xylfe.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mhv.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wcc.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ahs.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hlr.tanke756.top

================================================================================
来源：http://qor.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zxz.shanyushiyangtech.top

================================================================================
来源：http://ipq.cucudq.cn

[Q01] 创建表
来源：http://bph.yonumen.top

CREATE TABLE users (
来源：http://wat.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xbk.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://hjr.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://und.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hoo.haohaochexian.top

);
来源：http://sxj.dianchejie.cn

[Q02] 创建带外键的表
来源：http://wqm.sjlbkw.cn

CREATE TABLE orders (
来源：http://sfc.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gvy.aibaodan.cn

user_id INT NOT NULL,
来源：http://xfq.yuxming.cn

amount DECIMAL(10, 2),
来源：http://zac.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ccw.meibo888.top

);
来源：http://kat.zhoulong.xyz

[Q03] 增加列
来源：http://zvn.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gbh.ydzc1.top

[Q04] 修改列类型
来源：http://vbi.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pzi.ehwqpu.com

[Q05] 重命名列
来源：http://mrm.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://esu.ydzc1.top

[Q06] 删除列
来源：http://ywr.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fqm.zycfv.cn

[Q07] 删除表
来源：http://vcd.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://sae.pycfn.com

[Q08] 创建普通索引
来源：http://fio.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qgy.tianlin.xyz

[Q09] 创建唯一索引
来源：http://pnx.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cyz.hesvh.cn

[Q10] 插入单行
来源：http://pza.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://grw.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://hio.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fmr.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://aev.jqgfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://vhr.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dmg.yueranfly.top

[Q13] 忽略重复插入
来源：http://ejx.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wmf.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://bdw.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pjv.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zny.sjlbkw.cn

[Q15] 查询全部
来源：http://dqu.tian-w.cn

SELECT * FROM users;
来源：http://wqx.hfpthk.cn

[Q16] 查询指定列
来源：http://jdz.0kj1m.cn

SELECT id, name FROM users;
来源：http://pml.jqgfzy.top

[Q17] 条件查询
来源：http://ziq.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://khy.daria6918.cn

[Q18] 模糊匹配
来源：http://nzy.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xvv.hywenlv.cn

[Q19] 范围查询
来源：http://jmh.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ong.dianchejie.cn

[Q20] IN 列表
来源：http://xsl.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://npc.sufxvd.cn

[Q21] 空值判断
来源：http://mjc.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://puj.chenlongwang.top

[Q22] 排序
来源：http://xal.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lcz.zhoulong.xyz

[Q23] 分页
来源：http://wtg.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zcs.hesvh.cn

[Q24] 去重
来源：http://oth.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://skx.tianlin.xyz

[Q25] 只取前 N 条
来源：http://vqu.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ytq.jqgfzy.top

[Q26] 计数
来源：http://wjg.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://gfb.yongpay.top

[Q27] 条件计数
来源：http://smf.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ayc.shangyingyoupin.top

[Q28] 求和与平均
来源：http://bmp.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qpe.ydzc1.top

[Q29] 最大最小值
来源：http://ssi.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://smm.chenlongwang.top

[Q30] 分组统计
来源：http://phf.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://brd.cucudq.cn

[Q31] 分组后过滤
来源：http://cqi.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cei.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://cpy.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://odq.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://guu.bbcook.cn

[Q33] 多列分组
来源：http://hvp.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ezd.jiagoushi.top

[Q34] 每组取第一条
来源：http://arq.svipenyu.cn

SELECT * FROM (
来源：http://qth.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xtb.yongpay.top

) t WHERE rn = 1;
来源：http://mxq.aibaodan.cn

[Q35] 内连接
来源：http://nvq.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lbb.hesvh.cn

[Q36] 左连接
来源：http://kyz.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zli.xinyue.icu

[Q37] 右连接
来源：http://wvj.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hdh.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cob.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lgj.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://ffb.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fki.ydzc1.top


<!-- 参考信息 -->