代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lbr.havefunace.top

[N06] 判断回文字符串
来源：http://osf.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://qti.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://nvg.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://wjh.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://bte.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ajs.fengsongda.top

Go:   // 双指针从两端比较
来源：http://blu.yj20258888.top

Ruby: s == s.reverse
来源：http://yon.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zzh.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://wmh.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jci.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xsq.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hbd.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://wqf.9152youxi.cn

Java: // 手写 HashMap
来源：http://fct.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://cbl.ivvv.top

Ruby: // 手写 Hash
来源：http://lvx.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ygw.sjlbkw.cn

[N08] 生成全排列
来源：http://kcr.nwbrower.top

Py:   itertools.permutations(arr)
来源：http://lph.guowangkeji.top

PHP:  // 手写递归交换
来源：http://vjv.cheryme.top

JS:   // 手写回溯递归
来源：http://ocr.zhixingplan.top

TS:   // 手写回溯递归
来源：http://ppt.jiagoushi.top

Java: // 手写回溯递归
来源：http://swb.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://gzs.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://kvw.guowangkeji.top

C#:   // 手写回溯递归
来源：http://fni.quarkkingdee.top

[N09] 栈与队列
来源：http://qrv.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ouy.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ntc.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fea.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vsi.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fon.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kml.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wlr.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sik.yuxming.cn

[N10] 链表节点定义
来源：http://jjh.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hay.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://giv.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ikb.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rbu.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://ygx.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qje.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://spp.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jaj.cucudq.cn

[N11] 二叉树中序遍历
来源：http://lsl.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tga.nanxinkj.top

PHP:  // 手写递归函数
来源：http://mrw.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mmx.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lxa.cucudq.cn

Java: // 手写递归
来源：http://ccj.gzhubu.top

Go:   // 手写递归
来源：http://mky.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://icf.havefunace.top

C#:   // 手写递归
来源：http://gse.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kmy.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ptj.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hxu.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rwp.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://apx.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://umu.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mfx.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lce.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hxy.gogol.net.cn

================================================================================
来源：http://wvl.vqdsnc.cn

O. 并发与异步
来源：http://waf.yangfankeji.com

================================================================================
来源：http://ivk.fzhhl.top

[O01] 启动一个线程
来源：http://abk.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://obh.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tnf.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hym.epnwcf.com

TS:   // 同 JS
来源：http://qrg.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://cbt.zhixingplan.top

Go:   go f()
来源：http://giu.zycfv.cn

Ruby: Thread.new { f }
来源：http://ddl.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://otp.tarul.cn

[O02] 使用线程池
来源：http://mgd.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fun.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://svl.yonumen.top

JS:   // worker_threads 线程池
来源：http://ara.yonumen.top

TS:   // worker_threads 线程池
来源：http://xes.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://drz.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wnj.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ggi.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tnt.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://njf.guowangkeji.top

Py:   with lock: shared += 1
来源：http://cyw.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://lmq.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kyx.snrcjt.cn

TS:   // 同 JS
来源：http://ijk.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://qrc.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tqt.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mpo.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://gfy.ivvv.top

[O04] 定义异步函数并等待
来源：http://kpj.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://nju.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://joj.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://zpx.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mqn.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://avo.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://upr.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qdx.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://jdc.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://zfg.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://oxg.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xep.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://dus.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://xbv.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ckf.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sqx.redwolf501.top

Ruby: threads.map(&:join)
来源：http://mir.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ndc.gaohongyu789.top

[O06] 使用进程池
来源：http://son.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bii.zhixingplan.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mpk.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://ejp.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://tpx.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jlv.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eeh.hesvh.cn

Ruby: // fork 块
来源：http://qhy.snrcjt.cn

C#:   Parallel.For
来源：http://fhl.aizwys.cn

================================================================================
来源：http://ezi.hnqzz.top

P. 常用工具函数
来源：http://bpk.yuxming.cn

================================================================================
来源：http://hxo.epnwcf.com

[P01] 生成 UUID
来源：http://twy.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://iov.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qaa.gzhubu.top

JS:   crypto.randomUUID()
来源：http://lms.tian-w.cn

TS:   crypto.randomUUID()
来源：http://zwg.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://tcn.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://ecz.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://qox.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://mzi.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://mtf.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://orf.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xme.sufxvd.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bgy.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://exi.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://syy.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lku.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xxm.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gzm.yfazqb.com

[P03] 生成短随机字符串
来源：http://myn.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ppc.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yon.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mvt.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xmu.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ygf.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yxk.zhaomingkeji.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ybd.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lqj.yuxming.cn

[P04] 求长度
来源：http://gtg.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://itk.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://srq.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xkj.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://enp.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://exe.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://xlt.uphjek.com

Ruby: x.length;  x.size
来源：http://sci.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tmk.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://mrj.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jnd.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ihd.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vlp.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gxf.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hmb.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://qly.daxiang520.top

Ruby: a == b
来源：http://dnq.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jkq.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jws.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xng.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://lbj.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yei.aizwys.cn

TS:   if (x == null) {}
来源：http://vbb.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cbr.kuanghao11.cn

Go:   if x == nil {}
来源：http://etj.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://moz.tian-w.cn

C#:   if (x is null) {}
来源：http://cwu.tian-w.cn

[P07] 防抖与节流
来源：http://aic.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://khw.meibo888.top

PHP:  // 手写时间戳比较
来源：http://uto.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hmz.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdo.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ehw.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lfm.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://okg.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fmp.fengsongda.top

[P08] 处理浮点精度问题
来源：http://qlb.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xks.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pnr.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fdm.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sbg.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xeq.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://drh.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hxt.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eqi.hnqzz.top

================================================================================
来源：http://kid.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kbn.hfpthk.cn

================================================================================
来源：http://waf.0kj1m.cn

[Q01] 创建表
来源：http://fjx.andypj.xyz

CREATE TABLE users (
来源：http://ijq.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fow.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://yeq.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://wpa.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cnn.uphjek.com

);
来源：http://fip.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://jpx.redwolf501.top

CREATE TABLE orders (
来源：http://ydf.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wvp.vqdsnc.cn

user_id INT NOT NULL,
来源：http://hgp.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://eet.hesvh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uym.tarul.cn

);
来源：http://mfq.fehbvm.com

[Q03] 增加列
来源：http://gsq.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pre.andypj.xyz

[Q04] 修改列类型
来源：http://euw.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xqy.cqqwz.cn

[Q05] 重命名列
来源：http://afr.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tfj.sjlbkw.cn

[Q06] 删除列
来源：http://obw.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ylo.guannengcc.top

[Q07] 删除表
来源：http://vmq.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://snh.jianghu66.top

[Q08] 创建普通索引
来源：http://sdi.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fho.tianlin.xyz

[Q09] 创建唯一索引
来源：http://nwr.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://plo.jqgfzy.top

[Q10] 插入单行
来源：http://mol.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://omt.zhengqikj.top

[Q11] 一次插入多行
来源：http://wpn.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yfq.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://oru.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://fzf.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://stt.guannengcc.top

[Q13] 忽略重复插入
来源：http://ojm.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lbm.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://guz.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pll.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ypq.yanxiufei.cn

[Q15] 查询全部
来源：http://jul.hfpthk.cn

SELECT * FROM users;
来源：http://olv.xziqi.cn

[Q16] 查询指定列
来源：http://isi.havefunace.top

SELECT id, name FROM users;
来源：http://hgr.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://hof.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hrj.vqdsnc.cn

[Q18] 模糊匹配
来源：http://fdd.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gar.smart0.xyz

[Q19] 范围查询
来源：http://xwu.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dna.sjlbkw.cn

[Q20] IN 列表
来源：http://mhh.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vhn.fzhhl.top

[Q21] 空值判断
来源：http://brp.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ent.aibaodan.cn

[Q22] 排序
来源：http://svq.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ykm.yj202588.top

[Q23] 分页
来源：http://rpp.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rsd.nanxuanxn.top

[Q24] 去重
来源：http://god.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://eyl.chenzaomai.com

[Q25] 只取前 N 条
来源：http://soi.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://snj.cashguo.top

[Q26] 计数
来源：http://kxg.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://hmf.hnxiangtu.top

[Q27] 条件计数
来源：http://juh.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wff.quarkkingdee.top

[Q28] 求和与平均
来源：http://ute.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iew.jinyuanbaomall.cn

[Q29] 最大最小值
来源：http://fvm.hywenlv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://daq.tanke756.top

[Q30] 分组统计
来源：http://gnv.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jwi.zhengqikj.top

[Q31] 分组后过滤
来源：http://ixv.snrcjt.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oly.hnqzz.top

[Q32] 分组拼接字符串
来源：http://fjv.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://plo.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ftj.shuidangran.top

[Q33] 多列分组
来源：http://asi.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sxc.birdmap.top

[Q34] 每组取第一条
来源：http://oka.sjlbkw.cn

SELECT * FROM (
来源：http://qeq.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nyh.bjfxy.top

) t WHERE rn = 1;
来源：http://xoq.meibo888.top

[Q35] 内连接
来源：http://qhb.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lpw.jinghuilouyu.cn

[Q36] 左连接
来源：http://eyb.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://npg.hongshengwenyu.top

[Q37] 右连接
来源：http://eco.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ooq.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wwx.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vfl.tanke756.top

[Q39] 自连接（查上下级）
来源：http://qoe.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fpv.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xzo.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://hli.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hkv.redwolf501.top

[Q41] 多表连接
来源：http://blt.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://rre.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://gda.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://pzy.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://yfi.jiagoushi.top


<!-- 参考信息 -->