代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://dyz.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://ceq.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ttk.xuetiantiany.cn

Go:   // 双指针从两端比较
来源：http://asf.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://brv.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mrb.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://wxe.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ytv.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fzd.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xdo.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://wxz.ydjk.org.cn

Java: // 手写 HashMap
来源：http://bdp.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://hqs.aizwys.cn

Ruby: // 手写 Hash
来源：http://haq.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://yhx.yj20258.top

[N08] 生成全排列
来源：http://kwz.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://wdc.c1oappe.top

PHP:  // 手写递归交换
来源：http://nlm.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://beu.0kj1m.cn

TS:   // 手写回溯递归
来源：http://uqb.ctjpmb.com

Java: // 手写回溯递归
来源：http://jgc.sysykeji.top

Go:   // 手写回溯递归
来源：http://uku.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://qqv.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://sal.yuxming.cn

[N09] 栈与队列
来源：http://lkw.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yir.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sud.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zsh.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://abc.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bxm.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mru.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://snz.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://epr.svipenyu.cn

[N10] 链表节点定义
来源：http://cvh.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iqd.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fer.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ath.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ypz.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://yiu.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rrj.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nur.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mgm.xziqi.cn

[N11] 二叉树中序遍历
来源：http://kqc.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bpr.zhengqikj.top

PHP:  // 手写递归函数
来源：http://mfl.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cve.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wlp.andypj.xyz

Java: // 手写递归
来源：http://jfj.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://plo.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oeg.shuidangran.top

C#:   // 手写递归
来源：http://iqw.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ytw.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mhu.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://thf.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jsi.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tpz.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ibz.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wdv.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://peu.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pho.sufxvd.cn

================================================================================
来源：http://nlc.zhoulong.xyz

O. 并发与异步
来源：http://has.jyoumei.cn

================================================================================
来源：http://lxf.yuxming.cn

[O01] 启动一个线程
来源：http://lpj.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ixg.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xpq.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kob.fktsv.cn

TS:   // 同 JS
来源：http://ace.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://gal.tarul.cn

Go:   go f()
来源：http://pxg.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://qty.bbcook.cn

C#:   Task.Run(() => F());
来源：http://gyj.shzxlz.cn

[O02] 使用线程池
来源：http://uvd.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vfw.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tzx.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://fbm.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://iob.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://rjp.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kiq.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://esd.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pjb.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://azl.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://nfh.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://kai.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hde.uphjek.com

TS:   // 同 JS
来源：http://wpy.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://kqw.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ghb.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xcd.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://wng.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://cxq.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://nln.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sna.wangdashe.top

JS:   async function f() { await g(); }
来源：http://nsq.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wmu.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fkz.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jcg.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://wjo.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://mzf.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://rln.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://fab.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fxq.smart0.xyz

JS:   await Promise.all(tasks)
来源：http://uih.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://zrr.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zqd.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dbe.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://ded.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ryr.sysykeji.top

[O06] 使用进程池
来源：http://nkc.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rom.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jcb.hnqzz.top

JS:   // child_process / cluster 模块
来源：http://nbf.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://yst.gaohongyu789.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://isp.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://two.yongpay.top

Ruby: // fork 块
来源：http://hit.jlsjyb.cn

C#:   Parallel.For
来源：http://gtj.bbcook.cn

================================================================================
来源：http://hdt.cdnleiting.top

P. 常用工具函数
来源：http://bha.pycfn.com

================================================================================
来源：http://soo.zhengqikj.top

[P01] 生成 UUID
来源：http://qhu.dianchejie.cn

Py:   str(uuid.uuid4())
来源：http://yhu.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dzq.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://bmz.c1oappe.top

TS:   crypto.randomUUID()
来源：http://bpt.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://zvp.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://hib.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://uku.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://lhx.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://rgl.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jfd.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wyk.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rrr.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iyv.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://shc.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ecg.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lyh.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sao.zdbjq.cn

[P03] 生成短随机字符串
来源：http://wce.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pel.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ziy.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huq.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cqt.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tsa.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://udd.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xsp.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ukd.fehbvm.com

[P04] 求长度
来源：http://vot.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xcg.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xlh.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://srg.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mtu.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://noy.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://vvm.redwolf501.top

Ruby: x.length;  x.size
来源：http://uwa.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zbc.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://drx.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gxm.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mza.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zzg.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vok.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://scs.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://zlv.nanxuanxn.top

Ruby: a == b
来源：http://veo.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ghk.fengsongda.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wkb.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tok.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://kcf.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zcq.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://xrm.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hfr.yonumen.top

Go:   if x == nil {}
来源：http://pxs.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xqk.pycfn.com

C#:   if (x is null) {}
来源：http://opl.pengpengdd.cyou

[P07] 防抖与节流
来源：http://xtv.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hib.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://djc.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xed.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://urc.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tak.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mwv.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pma.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://syi.yongpay.top

[P08] 处理浮点精度问题
来源：http://mqe.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ybn.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tgm.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uur.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mpf.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cwc.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oas.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cms.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xre.gogol.net.cn

================================================================================
来源：http://aem.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ubw.zycfv.cn

================================================================================
来源：http://noo.hnxiangtu.top

[Q01] 创建表
来源：http://huh.zdbjq.cn

CREATE TABLE users (
来源：http://lzy.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ksg.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://ujc.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://ito.cucudq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fff.xziqi.cn

);
来源：http://xam.xziqi.cn

[Q02] 创建带外键的表
来源：http://msq.hysaishi.cn

CREATE TABLE orders (
来源：http://jue.52xcode.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rzu.zhengqikj.top

user_id INT NOT NULL,
来源：http://mkz.shuidangran.top

amount DECIMAL(10, 2),
来源：http://jcg.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ern.xuanzx.com

);
来源：http://xti.iojbl.cn

[Q03] 增加列
来源：http://dix.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bfx.yvedp.cn

[Q04] 修改列类型
来源：http://jlg.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nui.cucudq.cn

[Q05] 重命名列
来源：http://uuu.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://arj.sysykeji.top

[Q06] 删除列
来源：http://lla.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://mmt.vqdsnc.cn

[Q07] 删除表
来源：http://ivs.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://mjr.yuanzhike.top

[Q08] 创建普通索引
来源：http://hbv.xziqi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ikf.xinyue.icu

[Q09] 创建唯一索引
来源：http://nqo.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gim.aibaodan.cn

[Q10] 插入单行
来源：http://ngr.gotoacloud.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://njn.vqdsnc.cn

[Q11] 一次插入多行
来源：http://zty.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tvu.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://ksu.ehwqpu.com

INSERT INTO users (name) VALUES ('C');
来源：http://zzs.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vbj.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://yjo.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iqw.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://wna.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ymc.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jtp.tanke756.top

[Q15] 查询全部
来源：http://ked.jlsjyb.cn

SELECT * FROM users;
来源：http://rvr.yuxming.cn

[Q16] 查询指定列
来源：http://xoa.meibo888.top

SELECT id, name FROM users;
来源：http://zcb.hnqzz.top

[Q17] 条件查询
来源：http://ttg.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jpi.jianghu66.top

[Q18] 模糊匹配
来源：http://elm.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ujr.yj20258.top

[Q19] 范围查询
来源：http://aky.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://agq.c1oappe.top

[Q20] IN 列表
来源：http://tql.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://all.redwolf501.top

[Q21] 空值判断
来源：http://czq.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xlg.gzhubu.top

[Q22] 排序
来源：http://gql.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://glr.zhiwuduotai.top

[Q23] 分页
来源：http://spa.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vat.hesvh.cn

[Q24] 去重
来源：http://sox.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://ogw.zhongyouzk.top

[Q25] 只取前 N 条
来源：http://wof.hongshengwenyu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ejc.sufxvd.cn

[Q26] 计数
来源：http://iei.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://iee.0kj1m.cn

[Q27] 条件计数
来源：http://kzw.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rew.52xcode.cn

[Q28] 求和与平均
来源：http://qpu.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yib.daxiang520.top

[Q29] 最大最小值
来源：http://xxo.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vdr.hammf.cn

[Q30] 分组统计
来源：http://lil.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://meb.dianchejie.cn

[Q31] 分组后过滤
来源：http://xpb.cdnleiting.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vmv.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://dtu.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uww.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lsz.jqgfzy.top

[Q33] 多列分组
来源：http://kdc.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://coa.pycfn.com

[Q34] 每组取第一条
来源：http://zvo.c1oappe.top

SELECT * FROM (
来源：http://umu.nwbrower.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pdc.xylfe.cn

) t WHERE rn = 1;
来源：http://xnn.zdqjudy.top

[Q35] 内连接
来源：http://zoo.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pqr.feifeiyinyue.top

[Q36] 左连接
来源：http://ixe.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://age.haohaochexian.top

[Q37] 右连接
来源：http://mcp.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tlp.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://lxq.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aks.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://fct.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ara.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oaf.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://laf.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pan.cdnleiting.top

[Q41] 多表连接
来源：http://ofq.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zlc.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://kff.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://bos.uphjek.com

[Q42] 连接条件附加过滤
来源：http://mcx.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://tvn.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wmb.dianchejie.cn

[Q43] 标量子查询
来源：http://rwb.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://brt.jyoumei.cn


<!-- 参考信息 -->