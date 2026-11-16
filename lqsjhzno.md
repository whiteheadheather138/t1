代发 wailian999

[N05] 最大公约数
来源：http://ymm.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://jjn.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dwm.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wch.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lea.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bzf.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mbe.shzxlz.cn

Ruby: a.gcd(b)
来源：http://czu.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://seu.shuidangran.top

[N06] 判断回文字符串
来源：http://jke.zycfv.cn

Py:   s == s[::-1]
来源：http://dzc.52xcode.cn

PHP:  $s === strrev($s);
来源：http://jyw.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://aur.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://obt.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ady.andypj.xyz

Go:   // 双指针从两端比较
来源：http://sdz.cheryme.top

Ruby: s == s.reverse
来源：http://mld.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://luu.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://nbd.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qka.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oqv.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kps.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://dfn.iojbl.cn

Java: // 手写 HashMap
来源：http://iuk.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://tzl.cashguo.top

Ruby: // 手写 Hash
来源：http://udi.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cne.sufxvd.cn

[N08] 生成全排列
来源：http://ksl.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://pkv.pycfn.com

PHP:  // 手写递归交换
来源：http://ezy.yj202588.top

JS:   // 手写回溯递归
来源：http://esb.ivvv.top

TS:   // 手写回溯递归
来源：http://foq.shuidangran.top

Java: // 手写回溯递归
来源：http://rix.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://olq.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://bkm.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://ecc.pycfn.com

[N09] 栈与队列
来源：http://gam.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hbj.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pwr.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bcg.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bym.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zqj.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sya.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://avs.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nff.xziqi.cn

[N10] 链表节点定义
来源：http://fft.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ast.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cqx.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zbe.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://afa.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://ths.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://mqy.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ciq.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://egn.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://wjb.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xms.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://wrr.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tnh.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eua.nwbrower.top

Java: // 手写递归
来源：http://ocq.ivvv.top

Go:   // 手写递归
来源：http://vhv.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lal.hfpthk.cn

C#:   // 手写递归
来源：http://yex.zhiwuduotai.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iqi.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gtu.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uzz.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jqc.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bxi.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xjr.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://stf.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bcf.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dqv.jinghuilouyu.cn

================================================================================
来源：http://kvn.tanke756.top

O. 并发与异步
来源：http://oiv.tianlin.xyz

================================================================================
来源：http://gzj.zhiwuduotai.top

[O01] 启动一个线程
来源：http://scm.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zgr.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jij.hywenlv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ypi.shuidangran.top

TS:   // 同 JS
来源：http://msu.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://vfo.wangdashe.top

Go:   go f()
来源：http://tmm.yonumen.top

Ruby: Thread.new { f }
来源：http://kwr.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://ktm.jqgfzy.top

[O02] 使用线程池
来源：http://afp.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ltf.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://srm.fengsongda.top

JS:   // worker_threads 线程池
来源：http://mcy.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://yob.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://ooj.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fhp.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fcb.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jij.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://iba.haohaochexian.top

Py:   with lock: shared += 1
来源：http://rfl.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://imw.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rch.hnxiangtu.top

TS:   // 同 JS
来源：http://pni.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://saf.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dsg.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jpg.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://pnx.birdmap.top

[O04] 定义异步函数并等待
来源：http://qye.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://eev.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yvk.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://cds.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://bst.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pad.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kft.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://jtg.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://zqm.bbcook.cn

[O05] 并发执行并等待全部完成
来源：http://kqv.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://paa.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kvi.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://ksx.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://tqa.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ixj.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hxr.vehdjk.com

Ruby: threads.map(&:join)
来源：http://sgc.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://ysb.fktsv.cn

[O06] 使用进程池
来源：http://rvb.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sst.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vuo.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://wtz.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://mks.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ksy.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ogr.zdbjq.cn

Ruby: // fork 块
来源：http://bio.yj202588.top

C#:   Parallel.For
来源：http://stx.yangfankeji.com

================================================================================
来源：http://fly.aibaodan.cn

P. 常用工具函数
来源：http://wky.havefunace.top

================================================================================
来源：http://kjk.xziqi.cn

[P01] 生成 UUID
来源：http://mwe.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://xrk.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zak.pycfn.com

JS:   crypto.randomUUID()
来源：http://qvs.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://hbm.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://xpi.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://uvr.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://cmm.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://ksq.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://bor.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hxj.daria6918.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sue.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://clr.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iqk.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zvo.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dpd.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vac.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xoq.gzhubu.top

[P03] 生成短随机字符串
来源：http://vlr.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tch.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rbg.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vmc.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ezc.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://czu.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bhe.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://snu.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wba.pengpengdd.cyou

[P04] 求长度
来源：http://khu.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hqe.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bjk.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uhr.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fml.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://fja.snrcjt.cn

Go:   len(arr);  len(m)
来源：http://afd.daria6918.cn

Ruby: x.length;  x.size
来源：http://iwb.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vrq.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://zmw.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ywp.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hju.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uce.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hsl.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dlo.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://brx.gzhubu.top

Ruby: a == b
来源：http://ouw.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ids.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mvd.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tcw.316326.xyz

PHP:  if (empty($x)) {}
来源：http://etv.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bby.yj20258888.top

TS:   if (x == null) {}
来源：http://xdk.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rzt.gotoacloud.top

Go:   if x == nil {}
来源：http://knm.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://etk.dianchejie.cn

C#:   if (x is null) {}
来源：http://dur.hongshengwenyu.top

[P07] 防抖与节流
来源：http://yzn.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uhx.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://dmt.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wkz.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sng.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ngs.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ucn.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://int.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://upp.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://dma.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tmn.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iek.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://llg.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cex.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fai.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://epw.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lwh.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xpt.hesvh.cn

================================================================================
来源：http://ylb.zdbjq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vrz.zhengqikj.top

================================================================================
来源：http://kng.shangyingyoupin.top

[Q01] 创建表
来源：http://ylz.jqgfzy.top

CREATE TABLE users (
来源：http://mhu.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sqz.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://cyd.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://xco.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zrg.uphjek.com

);
来源：http://juw.sysykeji.top

[Q02] 创建带外键的表
来源：http://nad.uphjek.com

CREATE TABLE orders (
来源：http://iof.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gkm.nanxuanxn.top

user_id INT NOT NULL,
来源：http://rsc.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://mbu.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://euu.jinqigfzy.top

);
来源：http://rvl.hnqzz.top

[Q03] 增加列
来源：http://gjc.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ydz.ctjpmb.com

[Q04] 修改列类型
来源：http://qpy.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://amf.iojbl.cn

[Q05] 重命名列
来源：http://oml.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fkw.c1oappe.top

[Q06] 删除列
来源：http://kqe.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://bti.tanke756.top

[Q07] 删除表
来源：http://adf.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://zve.sweek.top

[Q08] 创建普通索引
来源：http://qko.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://jbp.hammf.cn

[Q09] 创建唯一索引
来源：http://wzr.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ydz.xylfe.cn

[Q10] 插入单行
来源：http://dvj.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uol.jinqigufen.top

[Q11] 一次插入多行
来源：http://wiz.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bvv.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://amz.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://gig.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://swm.yj20258888.top

[Q13] 忽略重复插入
来源：http://nsg.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://plg.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://rem.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rlp.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iyc.hnxiangtu.top

[Q15] 查询全部
来源：http://gou.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://omb.52xcode.cn

[Q16] 查询指定列
来源：http://nwn.daxiang520.top

SELECT id, name FROM users;
来源：http://rie.yangfankeji.com

[Q17] 条件查询
来源：http://dlu.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zyw.zdbjq.cn

[Q18] 模糊匹配
来源：http://odm.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rhg.tianlin.xyz

[Q19] 范围查询
来源：http://xnd.epnwcf.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gva.yongpay.top

[Q20] IN 列表
来源：http://nap.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oxe.sysykeji.top

[Q21] 空值判断
来源：http://uvc.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xzj.shzxlz.cn

[Q22] 排序
来源：http://zmp.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://coj.aibaodan.cn

[Q23] 分页
来源：http://qon.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yaf.ydzc1.top

[Q24] 去重
来源：http://ces.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://rzg.zhengqikj.top

[Q25] 只取前 N 条
来源：http://dkk.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xxt.yuanzhike.top

[Q26] 计数
来源：http://vog.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://pkf.nwbrower.top

[Q27] 条件计数
来源：http://dob.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ljz.jinqigufen.top

[Q28] 求和与平均
来源：http://rbv.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bcj.yuxming.cn

[Q29] 最大最小值
来源：http://btm.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ywf.shanyushiyangtech.top

[Q30] 分组统计
来源：http://gjk.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hwl.jqgufenzy.top

[Q31] 分组后过滤
来源：http://odi.cheryme.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jeh.yonumen.top

[Q32] 分组拼接字符串
来源：http://xfy.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://llb.zhengqikj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fga.mhx1999.top

[Q33] 多列分组
来源：http://iwc.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cet.gzhubu.top

[Q34] 每组取第一条
来源：http://vgs.tianlin.xyz

SELECT * FROM (
来源：http://opd.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ubc.yuanzhike.top

) t WHERE rn = 1;
来源：http://iiv.yj20258.top

[Q35] 内连接
来源：http://hpm.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bhi.sxryk.cn

[Q36] 左连接
来源：http://wga.0kj1m.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jdt.cheryme.top

[Q37] 右连接
来源：http://kew.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://woh.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://kox.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wop.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://vst.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yxz.jianghu66.top


<!-- 参考信息 -->