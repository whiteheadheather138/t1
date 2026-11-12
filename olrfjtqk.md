代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yer.ybcxt.top

[N06] 判断回文字符串
来源：http://hza.daria6918.cn

Py:   s == s[::-1]
来源：http://vja.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://mxd.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://ndq.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://llc.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ahb.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://rgu.zhongyouzk.top

Ruby: s == s.reverse
来源：http://lfb.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qbx.cheryme.top

[N07] 两数之和（返回下标）
来源：http://ifl.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xnp.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mhn.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hmj.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://vjw.jqgfzy.top

Java: // 手写 HashMap
来源：http://omh.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://azx.zycfv.cn

Ruby: // 手写 Hash
来源：http://jad.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ewo.jlsjyb.cn

[N08] 生成全排列
来源：http://hoa.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://vbk.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://fcy.yueranfly.top

JS:   // 手写回溯递归
来源：http://xvk.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://rpr.sysykeji.top

Java: // 手写回溯递归
来源：http://aeo.pycfn.com

Go:   // 手写回溯递归
来源：http://gnb.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://mnb.jqgfzy.top

C#:   // 手写回溯递归
来源：http://hwm.yangfankeji.com

[N09] 栈与队列
来源：http://uzf.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://trx.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wol.shuidangran.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iya.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vbg.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kzs.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gzu.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jhd.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wbo.dianchejie.cn

[N10] 链表节点定义
来源：http://jfj.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wot.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ofg.chenzaomai.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iiu.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ifl.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://hwm.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://kqy.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ejy.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yse.ctjpmb.com

[N11] 二叉树中序遍历
来源：http://cih.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ogx.xingfuxueyuan.xyz

PHP:  // 手写递归函数
来源：http://uxn.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bbo.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wqz.birdmap.top

Java: // 手写递归
来源：http://cgo.yanxiufei.cn

Go:   // 手写递归
来源：http://auz.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lmy.yanxiufei.cn

C#:   // 手写递归
来源：http://xxa.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://skn.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dox.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wfx.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xfh.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqx.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://afe.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tkd.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lph.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tzk.yonumen.top

================================================================================
来源：http://gea.c1oappe.top

O. 并发与异步
来源：http://ino.havefunace.top

================================================================================
来源：http://bvl.zhixingplan.top

[O01] 启动一个线程
来源：http://cgb.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tkh.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jii.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ynl.gaohongyu789.top

TS:   // 同 JS
来源：http://nar.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://ohr.gotoacloud.top

Go:   go f()
来源：http://kjo.vehdjk.com

Ruby: Thread.new { f }
来源：http://wak.yueranfly.top

C#:   Task.Run(() => F());
来源：http://vix.vqdsnc.cn

[O02] 使用线程池
来源：http://mgp.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rvb.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xef.c1oappe.top

JS:   // worker_threads 线程池
来源：http://gwn.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://giz.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://jxc.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tug.sxryk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jeg.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ogv.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://zul.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://nvp.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://chu.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zei.cheryme.top

TS:   // 同 JS
来源：http://qww.jlsjyb.cn

Java: synchronized (this) { shared++; }
来源：http://dqv.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nzu.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ycy.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://sby.yj20258.top

[O04] 定义异步函数并等待
来源：http://ovd.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://khf.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blv.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://jmi.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://ypm.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ebq.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lsw.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://olx.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://qqh.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://mvh.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://vpp.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cde.316326.xyz

JS:   await Promise.all(tasks)
来源：http://qpi.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://jmp.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ecp.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://txe.cucudq.cn

Ruby: threads.map(&:join)
来源：http://upn.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xfa.jyoumei.cn

[O06] 使用进程池
来源：http://mds.zhengqikj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ojr.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zds.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://hdq.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://law.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nqb.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zii.sweek.top

Ruby: // fork 块
来源：http://jmb.wangdashe.top

C#:   Parallel.For
来源：http://tvn.sjlbkw.cn

================================================================================
来源：http://ugk.xuanzx.com

P. 常用工具函数
来源：http://hdb.xylfe.cn

================================================================================
来源：http://vrq.yanxiufei.cn

[P01] 生成 UUID
来源：http://wbi.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://ago.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xol.andypj.xyz

JS:   crypto.randomUUID()
来源：http://xvp.havefunace.top

TS:   crypto.randomUUID()
来源：http://elj.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://pvl.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://dxh.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://rfn.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://yrs.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://nwe.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qqv.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dtd.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xoy.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dda.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wfw.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dhg.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nrc.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xkc.gogol.net.cn

[P03] 生成短随机字符串
来源：http://xik.jinqigfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wec.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fbu.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qnd.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sft.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://whk.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mvb.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://unu.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bpc.9152youxi.cn

[P04] 求长度
来源：http://sve.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pko.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mwp.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hps.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lup.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://ycc.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://hbm.havefunace.top

Ruby: x.length;  x.size
来源：http://voo.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jrm.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://qzr.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sox.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nvt.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oaf.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://afl.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://moo.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://oet.guowangkeji.top

Ruby: a == b
来源：http://ztt.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hru.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wmv.hywenlv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://emj.yj202588.top

PHP:  if (empty($x)) {}
来源：http://oir.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kal.guowangkeji.top

TS:   if (x == null) {}
来源：http://bus.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://dsp.bjfxy.top

Go:   if x == nil {}
来源：http://zdd.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nnm.yvedp.cn

C#:   if (x is null) {}
来源：http://ycd.vqdsnc.cn

[P07] 防抖与节流
来源：http://khi.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://paw.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://vwv.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rgy.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://php.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ltc.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vkk.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bwk.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ioc.aizwys.cn

[P08] 处理浮点精度问题
来源：http://lsy.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dfq.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sqd.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qel.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iyo.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jik.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nzv.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hbd.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jel.cucudq.cn

================================================================================
来源：http://cjg.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://grb.jianghu66.top

================================================================================
来源：http://ciy.andypj.xyz

[Q01] 创建表
来源：http://oyp.mhx1999.top

CREATE TABLE users (
来源：http://bje.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://daf.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://don.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://pth.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gez.ydjk.org.cn

);
来源：http://jcc.gotoacloud.top

[Q02] 创建带外键的表
来源：http://duy.tianlin.xyz

CREATE TABLE orders (
来源：http://oko.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eew.nanxinkj.top

user_id INT NOT NULL,
来源：http://dii.sysykeji.top

amount DECIMAL(10, 2),
来源：http://bpo.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bxo.jlsjyb.cn

);
来源：http://mzv.tarul.cn

[Q03] 增加列
来源：http://jlc.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://inm.haohaochexian.top

[Q04] 修改列类型
来源：http://zrg.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mnw.52xcode.cn

[Q05] 重命名列
来源：http://qgt.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xdv.sxryk.cn

[Q06] 删除列
来源：http://pac.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://gag.xuanzx.com

[Q07] 删除表
来源：http://nre.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://fgb.svipenyu.cn

[Q08] 创建普通索引
来源：http://wby.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fmh.dianchejie.cn

[Q09] 创建唯一索引
来源：http://mxp.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zyd.gotoacloud.top

[Q10] 插入单行
来源：http://lxc.sysykeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mqi.yj20258888.top

[Q11] 一次插入多行
来源：http://tla.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uxh.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://rxa.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://kce.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://edn.sysykeji.top

[Q13] 忽略重复插入
来源：http://dgn.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://efi.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://sjq.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vkj.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bwe.zhoulong.xyz

[Q15] 查询全部
来源：http://tvc.cqqwz.cn

SELECT * FROM users;
来源：http://emz.fehbvm.com

[Q16] 查询指定列
来源：http://pbs.dianchejie.cn

SELECT id, name FROM users;
来源：http://hqk.epnwcf.com

[Q17] 条件查询
来源：http://myv.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gqh.mhx1999.top

[Q18] 模糊匹配
来源：http://vrf.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://imp.zhaomingkeji.xyz

[Q19] 范围查询
来源：http://xvu.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eig.tianlin.xyz

[Q20] IN 列表
来源：http://xaw.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://koc.hammf.cn

[Q21] 空值判断
来源：http://vjd.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qcc.epnwcf.com

[Q22] 排序
来源：http://yce.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tpg.xuetiantiany.cn

[Q23] 分页
来源：http://duk.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hhy.zhixingplan.top

[Q24] 去重
来源：http://rdq.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://kek.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://wrx.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vta.redwolf501.top

[Q26] 计数
来源：http://goo.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://fio.xuanzx.com

[Q27] 条件计数
来源：http://btm.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vnx.yj20258.top

[Q28] 求和与平均
来源：http://vhu.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hkh.nwbrower.top

[Q29] 最大最小值
来源：http://dur.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wqz.zhongyouzk.top

[Q30] 分组统计
来源：http://pot.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pzs.sweek.top

[Q31] 分组后过滤
来源：http://vkm.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://csj.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://bvd.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nur.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xti.gotoacloud.top

[Q33] 多列分组
来源：http://jhh.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://otw.xziqi.cn

[Q34] 每组取第一条
来源：http://pnq.tian-w.cn

SELECT * FROM (
来源：http://enl.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iat.guowangkeji.top

) t WHERE rn = 1;
来源：http://cjd.hysaishi.cn

[Q35] 内连接
来源：http://gwh.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://etj.sxryk.cn

[Q36] 左连接
来源：http://ymr.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xof.cashguo.top

[Q37] 右连接
来源：http://tot.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rzz.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://leb.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zdf.pycfn.com

[Q39] 自连接（查上下级）
来源：http://hhq.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gbh.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fqn.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://irb.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://voq.hongshengwenyu.top

[Q41] 多表连接
来源：http://sfl.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://gmd.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://kfo.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://ncr.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://vpj.jqgfzy.top


<!-- 参考信息 -->