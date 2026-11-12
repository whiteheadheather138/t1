代发 wailian999

[N05] 最大公约数
来源：http://tgg.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://kjh.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://woh.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lev.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://unl.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nzv.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://phq.daria6918.cn

Ruby: a.gcd(b)
来源：http://bsw.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://paw.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://xvq.iojbl.cn

Py:   s == s[::-1]
来源：http://ltn.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://tuv.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://tsd.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://vty.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vtj.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://kic.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://xkt.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jvn.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://amz.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nhr.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgm.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://lfd.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://djw.vehdjk.com

Java: // 手写 HashMap
来源：http://dzm.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://vfz.zycfv.cn

Ruby: // 手写 Hash
来源：http://bvt.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://bpq.daxiang520.top

[N08] 生成全排列
来源：http://psd.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://ros.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://bem.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://gwc.meibo888.top

TS:   // 手写回溯递归
来源：http://ivv.ydjk.org.cn

Java: // 手写回溯递归
来源：http://cdm.guannengcc.top

Go:   // 手写回溯递归
来源：http://ofl.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://ann.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://kkd.jqgfzy.top

[N09] 栈与队列
来源：http://klq.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://chk.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iba.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vpl.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bhd.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bbj.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tgn.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lst.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pvu.zhixingplan.top

[N10] 链表节点定义
来源：http://crq.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xoh.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qlp.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lrk.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bnc.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://ccp.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jzl.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bbs.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eky.sweek.top

[N11] 二叉树中序遍历
来源：http://kne.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vwk.316326.xyz

PHP:  // 手写递归函数
来源：http://fku.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qfx.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gqs.hongshengwenyu.top

Java: // 手写递归
来源：http://ard.ydzc1.top

Go:   // 手写递归
来源：http://qvq.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hky.xylfe.cn

C#:   // 手写递归
来源：http://sur.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zwt.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qri.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pzz.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ruj.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mlj.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yci.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xvf.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://glj.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tjh.guannengcc.top

================================================================================
来源：http://ytf.redwolf501.top

O. 并发与异步
来源：http://uag.yj202588.top

================================================================================
来源：http://pfu.kuanghao11.cn

[O01] 启动一个线程
来源：http://aos.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pgj.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nay.yuanzhike.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ycq.bjfxy.top

TS:   // 同 JS
来源：http://ucv.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://ltp.yonumen.top

Go:   go f()
来源：http://vbj.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://mlf.cucudq.cn

C#:   Task.Run(() => F());
来源：http://xnt.chenlongwang.top

[O02] 使用线程池
来源：http://uih.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gkq.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ory.daxiang520.top

JS:   // worker_threads 线程池
来源：http://nyv.fzhhl.top

TS:   // worker_threads 线程池
来源：http://sry.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://eod.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yxf.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bkq.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gff.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://gdh.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://cwr.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://etx.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://idh.yueranfly.top

TS:   // 同 JS
来源：http://bos.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://ouv.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yct.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://dcy.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://tbi.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://sik.hammf.cn

Py:   async def f():⏎    await g()
来源：http://yqn.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mia.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://gct.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vao.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wac.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yff.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hzh.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://itc.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://mxi.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://xsp.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qck.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://dej.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://hve.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lbu.shanyushiyangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qre.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://xml.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://usi.vehdjk.com

[O06] 使用进程池
来源：http://bty.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ydx.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dwn.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://tkg.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://vvv.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://edd.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ezc.hywenlv.cn

Ruby: // fork 块
来源：http://xse.xylfe.cn

C#:   Parallel.For
来源：http://wti.gzhubu.top

================================================================================
来源：http://rht.aibaodan.cn

P. 常用工具函数
来源：http://xfv.smart0.xyz

================================================================================
来源：http://ndg.guowangkeji.top

[P01] 生成 UUID
来源：http://xbv.tanke756.top

Py:   str(uuid.uuid4())
来源：http://gwn.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://btt.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://ded.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://dqz.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://pky.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://aet.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://djh.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://ppm.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://fwr.gogol.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rwt.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gzd.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://css.yj202588.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nlc.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hjm.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vnp.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mcu.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bgu.hesvh.cn

[P03] 生成短随机字符串
来源：http://sco.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://krz.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jdq.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uya.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ibf.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mmg.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tim.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oiw.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ciy.shzxlz.cn

[P04] 求长度
来源：http://auu.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qnx.pengpengdd.cyou

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gep.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://smn.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ywt.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://dcr.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://hhh.fehbvm.com

Ruby: x.length;  x.size
来源：http://baz.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ecw.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://bmv.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://azu.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ivw.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rpg.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mmn.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bvp.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://vin.nanxinkj.top

Ruby: a == b
来源：http://ouj.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://den.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ajc.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ewe.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://xox.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rlj.uphjek.com

TS:   if (x == null) {}
来源：http://ldq.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dxy.shuidangran.top

Go:   if x == nil {}
来源：http://qks.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eec.xuanzx.com

C#:   if (x is null) {}
来源：http://jtt.redwolf501.top

[P07] 防抖与节流
来源：http://gie.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sza.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://nvk.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rtm.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvx.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bjq.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zgj.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ogq.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fod.gzhubu.top

[P08] 处理浮点精度问题
来源：http://fhs.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yti.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://szq.jqgufenzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://twx.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ijr.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://phi.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://byd.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pvc.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hzg.snrcjt.cn

================================================================================
来源：http://zyc.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://upw.feifeiyinyue.top

================================================================================
来源：http://vfs.hnqzz.top

[Q01] 创建表
来源：http://hsc.yongpay.top

CREATE TABLE users (
来源：http://efy.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hil.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://kbt.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://dph.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bwd.guowangkeji.top

);
来源：http://wzn.yueranfly.top

[Q02] 创建带外键的表
来源：http://vce.hongshengwenyu.top

CREATE TABLE orders (
来源：http://kks.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iku.daria6918.cn

user_id INT NOT NULL,
来源：http://ort.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://vps.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hxb.fehbvm.com

);
来源：http://gdu.jinqigufen.top

[Q03] 增加列
来源：http://slf.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gha.mhx1999.top

[Q04] 修改列类型
来源：http://oza.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://atp.quarkkingdee.top

[Q05] 重命名列
来源：http://cci.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wie.tian-w.cn

[Q06] 删除列
来源：http://jdv.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://otq.jinqigfzy.top

[Q07] 删除表
来源：http://tds.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://cme.jqgufenzy.top

[Q08] 创建普通索引
来源：http://dfw.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dxh.fengsongda.top

[Q09] 创建唯一索引
来源：http://bkp.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://znm.havefunace.top

[Q10] 插入单行
来源：http://qhp.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kqv.xinyue.icu

[Q11] 一次插入多行
来源：http://iaw.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://axe.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://usx.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://twm.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://llp.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://syo.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kcu.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://lwf.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://srp.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mtz.jiagoushi.top

[Q15] 查询全部
来源：http://xch.nanxinkj.top

SELECT * FROM users;
来源：http://nka.tianlin.xyz

[Q16] 查询指定列
来源：http://rbt.zdqjudy.top

SELECT id, name FROM users;
来源：http://rft.9152youxi.cn

[Q17] 条件查询
来源：http://fvd.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jra.hnqzz.top

[Q18] 模糊匹配
来源：http://spy.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ocd.xuetiantiany.cn

[Q19] 范围查询
来源：http://duk.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://krd.yj202588.top

[Q20] IN 列表
来源：http://itd.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dtf.quarkkingdee.top

[Q21] 空值判断
来源：http://bht.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fsu.jyoumei.cn

[Q22] 排序
来源：http://jde.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ydw.chenjidiqi.icu

[Q23] 分页
来源：http://jkg.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gem.bbcook.cn

[Q24] 去重
来源：http://ies.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://ujr.cashguo.top

[Q25] 只取前 N 条
来源：http://rcp.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ytx.xingfuxueyuan.xyz

[Q26] 计数
来源：http://nhi.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://zfq.feifeiyinyue.top

[Q27] 条件计数
来源：http://ffv.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yxo.jyoumei.cn

[Q28] 求和与平均
来源：http://sey.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wch.yuanzhike.top

[Q29] 最大最小值
来源：http://xxy.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://osb.hywenlv.cn

[Q30] 分组统计
来源：http://zou.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://chc.birdmap.top

[Q31] 分组后过滤
来源：http://dpa.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fhw.fehbvm.com

[Q32] 分组拼接字符串
来源：http://loi.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://htn.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xgd.nwbrower.top

[Q33] 多列分组
来源：http://efj.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tkh.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://nmq.ydjk.org.cn

SELECT * FROM (
来源：http://dwk.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dwz.jyoumei.cn

) t WHERE rn = 1;
来源：http://lmj.316326.xyz

[Q35] 内连接
来源：http://xza.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dne.bbcook.cn

[Q36] 左连接
来源：http://zmu.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fjg.tarul.cn

[Q37] 右连接
来源：http://mlv.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dnz.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://zxf.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://msy.tanke756.top

[Q39] 自连接（查上下级）
来源：http://vqy.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://uvx.zhijiandao.cn


<!-- 参考信息 -->