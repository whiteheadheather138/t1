代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gbj.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qfw.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://izj.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwo.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tde.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lzb.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xok.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://idw.ydjk.org.cn

[N05] 最大公约数
来源：http://dxq.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://kds.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uzk.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qgk.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qbv.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://djg.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://roi.chenzaomai.com

Ruby: a.gcd(b)
来源：http://nzq.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ism.ydjk.org.cn

[N06] 判断回文字符串
来源：http://lhv.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://lib.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://ybq.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://uqn.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://leo.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aas.aizwys.cn

Go:   // 双指针从两端比较
来源：http://pph.yonumen.top

Ruby: s == s.reverse
来源：http://ztp.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qwq.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://pvp.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xpu.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vei.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tpv.chenzaomai.com

TS:   // 手写 Map<string, number>
来源：http://hzw.zhixingplan.top

Java: // 手写 HashMap
来源：http://shz.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://evr.jyoumei.cn

Ruby: // 手写 Hash
来源：http://deh.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xkz.yj20258.top

[N08] 生成全排列
来源：http://fbg.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://ijk.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://axm.guowangkeji.top

JS:   // 手写回溯递归
来源：http://wjb.hcnkem.com

TS:   // 手写回溯递归
来源：http://lhv.yongpay.top

Java: // 手写回溯递归
来源：http://xos.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://sph.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://eqf.bjfxy.top

C#:   // 手写回溯递归
来源：http://rlf.c1oappe.top

[N09] 栈与队列
来源：http://hzy.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vss.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lly.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oif.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tbm.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zwx.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wrq.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wnl.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://emw.fzhhl.top

[N10] 链表节点定义
来源：http://ytu.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sue.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zov.jianghu66.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://poa.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://luk.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://abr.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://ftq.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://olk.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ilw.ybcxt.top

[N11] 二叉树中序遍历
来源：http://npn.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://opz.gzhubu.top

PHP:  // 手写递归函数
来源：http://lhm.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hez.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vvk.cdnleiting.top

Java: // 手写递归
来源：http://gwl.andypj.xyz

Go:   // 手写递归
来源：http://nxy.gotoacloud.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yxt.gotoacloud.top

C#:   // 手写递归
来源：http://ueo.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kcr.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iyl.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xtj.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hnr.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yfa.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fli.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yfi.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nrg.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://suv.yueranfly.top

================================================================================
来源：http://kyp.zhoulong.xyz

O. 并发与异步
来源：http://whw.xuanzx.com

================================================================================
来源：http://rcb.hywenlv.cn

[O01] 启动一个线程
来源：http://obo.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://keg.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xss.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tnx.meibo888.top

TS:   // 同 JS
来源：http://kyu.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://nqi.guowangkeji.top

Go:   go f()
来源：http://swc.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://gzn.fehbvm.com

C#:   Task.Run(() => F());
来源：http://udy.tarul.cn

[O02] 使用线程池
来源：http://hyn.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pxd.zhijiandao.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jxo.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://etz.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://sly.tarul.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ghh.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lon.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kdx.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nlz.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://ngk.quarkkingdee.top

Py:   with lock: shared += 1
来源：http://vbc.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://clf.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sxh.jinqigufen.top

TS:   // 同 JS
来源：http://rzr.gogol.net.cn

Java: synchronized (this) { shared++; }
来源：http://iea.tian-w.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://drz.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ckj.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://msn.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://wyc.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://otw.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lai.xylfe.cn

JS:   async function f() { await g(); }
来源：http://mbu.jyoumei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pou.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sih.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xzb.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://vpx.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://bcm.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://ros.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://fke.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://snm.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://jub.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://fyw.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ujw.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uhb.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://cii.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://jwo.svipenyu.cn

[O06] 使用进程池
来源：http://fns.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fdj.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://glg.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://wyr.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://jrp.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xnn.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fis.zhixingplan.top

Ruby: // fork 块
来源：http://woz.guannengcc.top

C#:   Parallel.For
来源：http://anp.daria6918.cn

================================================================================
来源：http://eot.zdqjudy.top

P. 常用工具函数
来源：http://bzc.jinqigufen.top

================================================================================
来源：http://rtg.zhongyouzk.top

[P01] 生成 UUID
来源：http://lqq.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://rzn.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hiz.yonumen.top

JS:   crypto.randomUUID()
来源：http://qvk.vehdjk.com

TS:   crypto.randomUUID()
来源：http://hde.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://zua.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://hdm.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://dde.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://evx.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://oae.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ksg.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uba.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xlm.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yuh.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cys.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wkh.smart0.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fyl.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jqk.meibo888.top

[P03] 生成短随机字符串
来源：http://idj.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nib.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cvq.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ubl.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xms.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bsa.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mij.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lua.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lmy.ivvv.top

[P04] 求长度
来源：http://teo.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mhg.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cve.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ciy.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://arq.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://rgh.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://aro.guannengcc.top

Ruby: x.length;  x.size
来源：http://upc.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ara.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://nxg.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ykj.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jve.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xov.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sit.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xgo.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://cxp.daxiang520.top

Ruby: a == b
来源：http://alc.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tyx.zdqjudy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kud.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rhq.shuidangran.top

PHP:  if (empty($x)) {}
来源：http://vzb.yj202588.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vmh.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://zbc.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://soa.ywan-chungtsiang.top

Go:   if x == nil {}
来源：http://cix.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zbh.jinqigufen.top

C#:   if (x is null) {}
来源：http://pdk.xinyue.icu

[P07] 防抖与节流
来源：http://uux.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kpc.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://dck.bbcook.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cah.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kll.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dic.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://omp.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xmn.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rbm.yueranfly.top

[P08] 处理浮点精度问题
来源：http://yxy.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ovj.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://grp.zdbjq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wnf.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xcq.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rtl.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fye.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fzu.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fvq.yj20258.top

================================================================================
来源：http://lnm.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://npo.yj202588.top

================================================================================
来源：http://prv.yongpay.top

[Q01] 创建表
来源：http://ksp.pycfn.com

CREATE TABLE users (
来源：http://rci.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://giw.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://ehs.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://wus.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bcl.0kj1m.cn

);
来源：http://evv.fzhhl.top

[Q02] 创建带外键的表
来源：http://hwv.jianghu66.top

CREATE TABLE orders (
来源：http://cya.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zrf.xuanzx.com

user_id INT NOT NULL,
来源：http://cpb.hesvh.cn

amount DECIMAL(10, 2),
来源：http://hjk.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tyt.cucudq.cn

);
来源：http://mje.shanyushiyangkeji.top

[Q03] 增加列
来源：http://cee.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wgf.feifeiyinyue.top

[Q04] 修改列类型
来源：http://sfw.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cjq.wangdashe.top

[Q05] 重命名列
来源：http://npa.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ypy.yfazqb.com

[Q06] 删除列
来源：http://qim.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://qkj.yj202588.top

[Q07] 删除表
来源：http://rfv.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://kru.havefunace.top

[Q08] 创建普通索引
来源：http://lry.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mad.zhengqikj.top

[Q09] 创建唯一索引
来源：http://ubb.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hlj.yfazqb.com

[Q10] 插入单行
来源：http://cfj.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mgw.haohaochexian.top

[Q11] 一次插入多行
来源：http://pyg.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dei.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://wav.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://gdh.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fzq.zdqjudy.top

[Q13] 忽略重复插入
来源：http://fsx.aizwys.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xqj.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://ggh.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jfj.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ulj.shangyingyoupin.top

[Q15] 查询全部
来源：http://zlg.snrcjt.cn

SELECT * FROM users;
来源：http://mki.hnqzz.top

[Q16] 查询指定列
来源：http://sir.yvedp.cn

SELECT id, name FROM users;
来源：http://rsj.jianghu66.top

[Q17] 条件查询
来源：http://mez.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cec.sweek.top

[Q18] 模糊匹配
来源：http://hmz.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qhc.svipenyu.cn

[Q19] 范围查询
来源：http://eqk.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fmv.feifeiyinyue.top

[Q20] IN 列表
来源：http://yxq.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rhr.pengpengdd.cyou

[Q21] 空值判断
来源：http://xcj.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://umo.zdqjudy.top

[Q22] 排序
来源：http://nrf.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ahs.gaohongyu789.top

[Q23] 分页
来源：http://shj.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://brx.c1oappe.top

[Q24] 去重
来源：http://msz.xylfe.cn

SELECT DISTINCT city FROM users;
来源：http://eld.ehwqpu.com

[Q25] 只取前 N 条
来源：http://poo.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://may.fzhhl.top

[Q26] 计数
来源：http://uvv.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://knl.kuanghao11.cn

[Q27] 条件计数
来源：http://cse.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ofs.fzhhl.top

[Q28] 求和与平均
来源：http://kzv.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xgo.zhijiandao.cn

[Q29] 最大最小值
来源：http://hhw.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gso.yuanzhike.top

[Q30] 分组统计
来源：http://abc.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eub.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://juh.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xon.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://ebc.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jcd.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ntn.yueranfly.top

[Q33] 多列分组
来源：http://sys.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eoe.0kj1m.cn

[Q34] 每组取第一条
来源：http://rai.ppjwa.cn

SELECT * FROM (
来源：http://ikr.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cbr.cheryme.top

) t WHERE rn = 1;
来源：http://gan.vehdjk.com

[Q35] 内连接
来源：http://iox.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vkw.ivvv.top


<!-- 参考信息 -->