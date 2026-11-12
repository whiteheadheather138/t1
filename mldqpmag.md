代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kxx.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xcc.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://smk.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://zbi.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lmn.kuanghao11.cn

[N06] 判断回文字符串
来源：http://ior.zhijiandao.cn

Py:   s == s[::-1]
来源：http://dro.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://wjm.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://gdu.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://lic.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uzu.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://sme.9152youxi.cn

Ruby: s == s.reverse
来源：http://ett.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://vxo.meibo888.top

[N07] 两数之和（返回下标）
来源：http://opq.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wax.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kpe.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dps.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://bwk.xuanzx.com

Java: // 手写 HashMap
来源：http://urz.shuidangran.top

Go:   // 手写 map[int]int
来源：http://xdu.yonumen.top

Ruby: // 手写 Hash
来源：http://mtr.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://zgu.hnqzz.top

[N08] 生成全排列
来源：http://cwc.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://jlw.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://ekb.chenzaomai.com

JS:   // 手写回溯递归
来源：http://nbz.iojbl.cn

TS:   // 手写回溯递归
来源：http://xdf.hysaishi.cn

Java: // 手写回溯递归
来源：http://blt.aizwys.cn

Go:   // 手写回溯递归
来源：http://fdn.316326.xyz

Ruby: arr.permutation.to_a
来源：http://kyv.dashuyun.cn

C#:   // 手写回溯递归
来源：http://sfs.haohaochexian.top

[N09] 栈与队列
来源：http://vbn.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qih.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hbh.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cwh.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pmy.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mxi.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lyf.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://juo.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hkb.jianghu66.top

[N10] 链表节点定义
来源：http://chs.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ulg.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sjm.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jtm.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nns.tarul.cn

Java: class Node { int v; Node next; }
来源：http://bwg.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://crh.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sua.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xhh.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://woo.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wak.jiagoushi.top

PHP:  // 手写递归函数
来源：http://vsw.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yck.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gfn.haohaochexian.top

Java: // 手写递归
来源：http://ifc.andypj.xyz

Go:   // 手写递归
来源：http://qxv.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yuf.redwolf501.top

C#:   // 手写递归
来源：http://ulc.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nrf.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rwy.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dwq.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://neg.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tkk.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rnb.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nis.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bnu.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tyh.yuxming.cn

================================================================================
来源：http://dgs.0kj1m.cn

O. 并发与异步
来源：http://iqe.zhijiandao.cn

================================================================================
来源：http://znp.yuanzhike.top

[O01] 启动一个线程
来源：http://fhm.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vow.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zgs.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dde.hammf.cn

TS:   // 同 JS
来源：http://bxp.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://pvm.zhiwuduotai.top

Go:   go f()
来源：http://vss.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://kup.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://evg.yj202588.top

[O02] 使用线程池
来源：http://sgh.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qtc.tianlin.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hap.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://ste.jianghu66.top

TS:   // worker_threads 线程池
来源：http://tgz.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tgx.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oeh.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://int.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://odr.sysykeji.top

[O03] 加锁保护共享数据
来源：http://igf.guowangkeji.top

Py:   with lock: shared += 1
来源：http://uvd.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://wii.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nui.cashguo.top

TS:   // 同 JS
来源：http://bxr.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://qdj.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://agy.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lri.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://mda.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://jyu.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://lbp.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yuh.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://wqx.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nlq.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://odc.haohaochexian.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rsg.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://qwn.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://vqc.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://rur.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://khx.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eyb.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://sbe.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://vzl.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vus.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ndj.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://atk.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ycj.chenjidiqi.icu

[O06] 使用进程池
来源：http://ydm.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xma.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://dcl.316326.xyz

JS:   // child_process / cluster 模块
来源：http://jsy.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://bxc.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xuy.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kzu.chenzaomai.com

Ruby: // fork 块
来源：http://lri.haohaochexian.top

C#:   Parallel.For
来源：http://akr.guannengcc.top

================================================================================
来源：http://jyn.epnwcf.com

P. 常用工具函数
来源：http://zfc.yonumen.top

================================================================================
来源：http://yes.jinqigufen.top

[P01] 生成 UUID
来源：http://xjh.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://ztv.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mhc.yfazqb.com

JS:   crypto.randomUUID()
来源：http://iql.52xcode.cn

TS:   crypto.randomUUID()
来源：http://bji.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://zco.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://muh.yj202588.top

Ruby: SecureRandom.uuid
来源：http://ozu.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://pvh.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://vay.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eoa.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://swr.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tfn.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tmk.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://riz.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tyb.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://liu.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mmj.zycfv.cn

[P03] 生成短随机字符串
来源：http://gvd.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://imb.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vrs.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xbn.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ycm.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lii.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://agt.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iib.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sul.xziqi.cn

[P04] 求长度
来源：http://toy.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kki.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://myg.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jrp.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qtm.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://mnd.ydzc1.top

Go:   len(arr);  len(m)
来源：http://lnh.fengsongda.top

Ruby: x.length;  x.size
来源：http://rak.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bnu.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://rig.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oee.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://llf.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jpa.pengpengdd.cyou

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lit.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lfl.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://jeo.zhengqikj.top

Ruby: a == b
来源：http://abu.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zhg.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://luv.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nsy.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://wku.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ixz.fengsongda.top

TS:   if (x == null) {}
来源：http://tyh.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rpk.pengpengdd.cyou

Go:   if x == nil {}
来源：http://abh.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lho.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://dwt.chenlongwang.top

[P07] 防抖与节流
来源：http://kjy.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ntm.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://ytm.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vhg.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mta.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nsu.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zkz.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kwy.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pna.daxiang520.top

[P08] 处理浮点精度问题
来源：http://aep.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://msq.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kxo.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wvr.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pzw.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kgo.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://acs.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rok.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://byb.wangshuangyany.cn

================================================================================
来源：http://dku.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://htq.quarkkingdee.top

================================================================================
来源：http://avb.xuanzx.com

[Q01] 创建表
来源：http://zdp.yuanzhike.top

CREATE TABLE users (
来源：http://abh.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gau.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://yos.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://ygl.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ldw.ydjk.org.cn

);
来源：http://tsf.yj20258.top

[Q02] 创建带外键的表
来源：http://dhg.xuanzx.com

CREATE TABLE orders (
来源：http://zgf.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iga.xuanzx.com

user_id INT NOT NULL,
来源：http://nqt.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://leu.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kmh.sufxvd.cn

);
来源：http://zkg.chenjidiqi.icu

[Q03] 增加列
来源：http://yuk.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bkt.c1oappe.top

[Q04] 修改列类型
来源：http://hlx.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sje.yongpay.top

[Q05] 重命名列
来源：http://fee.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://std.yj20258.top

[Q06] 删除列
来源：http://orl.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://abw.9152youxi.cn

[Q07] 删除表
来源：http://wiw.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://tbj.cdnleiting.top

[Q08] 创建普通索引
来源：http://vdq.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://csl.jqgfzy.top

[Q09] 创建唯一索引
来源：http://nku.yangfankeji.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gzc.havefunace.top

[Q10] 插入单行
来源：http://pij.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ygy.jinqigfzy.top

[Q11] 一次插入多行
来源：http://vdm.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uol.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://csg.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://pdv.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eof.yj20258.top

[Q13] 忽略重复插入
来源：http://abw.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sxp.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://gsr.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wrm.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zss.hammf.cn

[Q15] 查询全部
来源：http://jor.52xcode.cn

SELECT * FROM users;
来源：http://yhg.tarul.cn

[Q16] 查询指定列
来源：http://jip.jqgufenzy.top

SELECT id, name FROM users;
来源：http://uas.dianchejie.cn

[Q17] 条件查询
来源：http://dgb.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yvl.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://zcy.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uhd.zhoulong.xyz

[Q19] 范围查询
来源：http://xdc.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fmu.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://mbs.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tij.jqgufenzy.top

[Q21] 空值判断
来源：http://xqi.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ful.zhongyouzk.top

[Q22] 排序
来源：http://qfu.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jar.vqdsnc.cn

[Q23] 分页
来源：http://nmv.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dox.yfazqb.com

[Q24] 去重
来源：http://qwe.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://tyb.52xcode.cn

[Q25] 只取前 N 条
来源：http://cen.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fnl.zycfv.cn

[Q26] 计数
来源：http://wap.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://ogd.ybcxt.top

[Q27] 条件计数
来源：http://izr.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://del.hywenlv.cn

[Q28] 求和与平均
来源：http://fok.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ztn.xuetiantiany.cn

[Q29] 最大最小值
来源：http://bnd.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mai.yongpay.top

[Q30] 分组统计
来源：http://sfj.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eop.havefunace.top

[Q31] 分组后过滤
来源：http://cim.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vdn.cucudq.cn

[Q32] 分组拼接字符串
来源：http://hsn.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pjf.chenjidiqi.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nwi.fanxiaobao.xyz

[Q33] 多列分组
来源：http://rvc.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pet.bbcook.cn

[Q34] 每组取第一条
来源：http://nqq.c1oappe.top

SELECT * FROM (
来源：http://hnj.cucudq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mvs.sysykeji.top

) t WHERE rn = 1;
来源：http://dwb.vehdjk.com

[Q35] 内连接
来源：http://xwe.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://myu.xylfe.cn

[Q36] 左连接
来源：http://vkv.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ima.guowangkeji.top

[Q37] 右连接
来源：http://iux.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dgw.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://alp.jianghu66.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lib.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://ljf.quarkkingdee.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jip.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://koy.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://gmb.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ebt.meibo888.top

[Q41] 多表连接
来源：http://ebl.ivvv.top


<!-- 参考信息 -->