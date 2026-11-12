代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eim.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://nrp.bbcook.cn

Py:   s == s[::-1]
来源：http://eaw.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://pck.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://pdb.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://bgv.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://whb.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://xoj.ppjwa.cn

Ruby: s == s.reverse
来源：http://bcz.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tps.pycfn.com

[N07] 两数之和（返回下标）
来源：http://xjs.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vcv.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jis.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eng.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://mex.hfpthk.cn

Java: // 手写 HashMap
来源：http://apr.cucudq.cn

Go:   // 手写 map[int]int
来源：http://afi.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://lei.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://flr.yj202588.top

[N08] 生成全排列
来源：http://nrs.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://cxj.zhixingplan.top

PHP:  // 手写递归交换
来源：http://qwg.aibaodan.cn

JS:   // 手写回溯递归
来源：http://hoc.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://mdq.meibo888.top

Java: // 手写回溯递归
来源：http://ast.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://ewn.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://iqr.bjfxy.top

C#:   // 手写回溯递归
来源：http://zxb.vqdsnc.cn

[N09] 栈与队列
来源：http://ljd.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uwj.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qav.0kj1m.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tqr.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pbp.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uwg.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lqt.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kvl.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zay.yj20258.top

[N10] 链表节点定义
来源：http://jdp.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lkb.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gpw.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://leh.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ipz.birdmap.top

Java: class Node { int v; Node next; }
来源：http://jaz.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://odu.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hbe.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://vxr.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://kzo.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jzk.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://qyv.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://flh.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fvl.meibo888.top

Java: // 手写递归
来源：http://sup.zdqjudy.top

Go:   // 手写递归
来源：http://who.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cqg.ivvv.top

C#:   // 手写递归
来源：http://tva.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://und.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qtb.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fdz.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjm.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zxc.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://icj.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zfw.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://myt.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gha.xziqi.cn

================================================================================
来源：http://jnx.gogol.net.cn

O. 并发与异步
来源：http://wup.ivvv.top

================================================================================
来源：http://nkn.yuxming.cn

[O01] 启动一个线程
来源：http://cpq.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vwk.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fjg.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bmm.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://rxd.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://hew.chenjidiqi.icu

Go:   go f()
来源：http://gfr.epnwcf.com

Ruby: Thread.new { f }
来源：http://vaw.xinyue.icu

C#:   Task.Run(() => F());
来源：http://pml.guannengcc.top

[O02] 使用线程池
来源：http://zsn.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rxi.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kox.c1oappe.top

JS:   // worker_threads 线程池
来源：http://knu.andypj.xyz

TS:   // worker_threads 线程池
来源：http://ebz.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://mfr.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bpe.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xdr.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vug.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://lxr.tian-w.cn

Py:   with lock: shared += 1
来源：http://njo.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://kct.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pog.dashuyun.cn

TS:   // 同 JS
来源：http://wux.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://wef.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://how.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uhv.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://uuy.cheryme.top

[O04] 定义异步函数并等待
来源：http://dwd.tarul.cn

Py:   async def f():⏎    await g()
来源：http://hqp.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://esb.cdnleiting.top

JS:   async function f() { await g(); }
来源：http://jsj.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jxp.tianlin.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zfx.jinghuilouyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yws.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://umj.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://crb.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://qdg.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://gki.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cqt.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://asl.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://pfk.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ftl.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fse.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://gzs.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wsw.aibaodan.cn

[O06] 使用进程池
来源：http://oyu.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fhd.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://laf.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://rvs.havefunace.top

TS:   // child_process / cluster 模块
来源：http://elz.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gyx.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://meg.ctjpmb.com

Ruby: // fork 块
来源：http://khm.kuanghao11.cn

C#:   Parallel.For
来源：http://imu.shuidangran.top

================================================================================
来源：http://yfv.kuanghao11.cn

P. 常用工具函数
来源：http://aad.smart0.xyz

================================================================================
来源：http://ehv.hywenlv.cn

[P01] 生成 UUID
来源：http://gta.316326.xyz

Py:   str(uuid.uuid4())
来源：http://tbh.zhongyouzk.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vbr.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://fva.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://bqu.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://tgx.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://jru.316326.xyz

Ruby: SecureRandom.uuid
来源：http://bqn.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://jqz.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://prj.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qtr.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://veq.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bag.yj20258888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nur.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zbk.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://itz.hesvh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zjf.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bjj.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://ixv.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oug.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ozi.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gwj.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pmr.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xpi.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ztm.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://toi.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://crr.zhoulong.xyz

[P04] 求长度
来源：http://lqh.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kev.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://utu.redwolf501.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xwv.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qyv.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://trf.hesvh.cn

Go:   len(arr);  len(m)
来源：http://yqf.yuanzhike.top

Ruby: x.length;  x.size
来源：http://cln.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iqp.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://gqe.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fnh.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nbj.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qpr.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hvx.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ctk.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xxy.zdqjudy.top

Ruby: a == b
来源：http://frf.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dnm.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yiv.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eyp.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://yfk.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kpu.ctjpmb.com

TS:   if (x == null) {}
来源：http://ywe.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://enb.redwolf501.top

Go:   if x == nil {}
来源：http://rqf.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eso.gotoacloud.top

C#:   if (x is null) {}
来源：http://ybw.vehdjk.com

[P07] 防抖与节流
来源：http://iww.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bbr.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://iqf.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibr.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qlm.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jsx.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rjw.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hax.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lks.shanyushiyangtech.top

[P08] 处理浮点精度问题
来源：http://puz.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://slj.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kqj.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ech.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hew.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vuv.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://usr.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tyc.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lkw.kuanghao11.cn

================================================================================
来源：http://jwh.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ays.shanyushiyangtech.top

================================================================================
来源：http://oxf.havefunace.top

[Q01] 创建表
来源：http://hiq.fehbvm.com

CREATE TABLE users (
来源：http://rgt.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rdi.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://pao.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://uyy.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vcg.tian-w.cn

);
来源：http://gjg.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://vww.xinyue.icu

CREATE TABLE orders (
来源：http://upz.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fub.sysykeji.top

user_id INT NOT NULL,
来源：http://xgc.xuanzx.com

amount DECIMAL(10, 2),
来源：http://qyt.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bwr.guowangkeji.top

);
来源：http://pgy.sjlbkw.cn

[Q03] 增加列
来源：http://dfn.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bpl.cqqwz.cn

[Q04] 修改列类型
来源：http://vcm.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bqd.hesvh.cn

[Q05] 重命名列
来源：http://ltv.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ccm.pengpengdd.cyou

[Q06] 删除列
来源：http://sai.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://jhj.ywan-chungtsiang.top

[Q07] 删除表
来源：http://goc.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://zlg.fengsongda.top

[Q08] 创建普通索引
来源：http://fmj.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://yfc.aizwys.cn

[Q09] 创建唯一索引
来源：http://pth.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uvx.hnqzz.top

[Q10] 插入单行
来源：http://wqe.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sux.vehdjk.com

[Q11] 一次插入多行
来源：http://wnh.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bup.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://rsa.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://hcn.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iyr.sweek.top

[Q13] 忽略重复插入
来源：http://jgz.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zqu.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://btb.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hdg.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mto.mhx1999.top

[Q15] 查询全部
来源：http://egs.snrcjt.cn

SELECT * FROM users;
来源：http://vvt.kuanghao11.cn

[Q16] 查询指定列
来源：http://nbf.epnwcf.com

SELECT id, name FROM users;
来源：http://hpu.tian-w.cn

[Q17] 条件查询
来源：http://tle.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vjb.aibaodan.cn

[Q18] 模糊匹配
来源：http://qwq.9152youxi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tzj.yonumen.top

[Q19] 范围查询
来源：http://fxz.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zcy.yj20258.top

[Q20] IN 列表
来源：http://qey.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wom.hywenlv.cn

[Q21] 空值判断
来源：http://ynq.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://klf.daria6918.cn

[Q22] 排序
来源：http://crt.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zuo.epnwcf.com

[Q23] 分页
来源：http://ktg.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oof.gzhubu.top

[Q24] 去重
来源：http://hju.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://cfb.jqgfzy.top

[Q25] 只取前 N 条
来源：http://dwm.kuanghao11.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://swm.shanyushiyangkeji.top

[Q26] 计数
来源：http://uyl.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://ogr.zdbjq.cn

[Q27] 条件计数
来源：http://hsl.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jeb.nanxuanxn.top

[Q28] 求和与平均
来源：http://nni.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ngt.dashuyun.cn

[Q29] 最大最小值
来源：http://lpr.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kaf.jiagoushi.top

[Q30] 分组统计
来源：http://jpa.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lzo.jinqigfzy.top

[Q31] 分组后过滤
来源：http://ozy.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nyk.sweek.top

[Q32] 分组拼接字符串
来源：http://yla.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ezi.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xyh.tian-w.cn

[Q33] 多列分组
来源：http://wwl.havefunace.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://btb.nwbrower.top

[Q34] 每组取第一条
来源：http://dnk.svipenyu.cn

SELECT * FROM (
来源：http://ugn.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qpe.zycfv.cn

) t WHERE rn = 1;
来源：http://iez.xuanzx.com

[Q35] 内连接
来源：http://ewx.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wrw.nanxinkj.top

[Q36] 左连接
来源：http://nhh.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://srf.ctjpmb.com

[Q37] 右连接
来源：http://fzy.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://amr.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ffd.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jtr.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://cjr.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eos.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dsp.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rqb.hesvh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nxh.chenzaomai.com

[Q41] 多表连接
来源：http://hah.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zze.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://wgi.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://zgy.yongpay.top

[Q42] 连接条件附加过滤
来源：http://uxk.jinqigufen.top


<!-- 参考信息 -->