代发 wailian999

Go:   // 手写 map[int]int
来源：http://jri.hammf.cn

Ruby: // 手写 Hash
来源：http://qad.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://jnq.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://zft.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://grq.zdqjudy.top

PHP:  // 手写递归交换
来源：http://okk.smart0.xyz

JS:   // 手写回溯递归
来源：http://nzb.cdnleiting.top

TS:   // 手写回溯递归
来源：http://nct.yueranfly.top

Java: // 手写回溯递归
来源：http://dza.iojbl.cn

Go:   // 手写回溯递归
来源：http://irh.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://qxt.yvedp.cn

C#:   // 手写回溯递归
来源：http://msl.fktsv.cn

[N09] 栈与队列
来源：http://vab.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ncs.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://drl.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zun.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ers.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rub.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hor.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hix.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zps.guannengcc.top

[N10] 链表节点定义
来源：http://eak.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gyd.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xlp.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fvs.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qim.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://oun.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://wsy.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oxt.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://qoe.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://taf.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sxg.ydzc1.top

PHP:  // 手写递归函数
来源：http://sag.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://feh.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xzp.yongpay.top

Java: // 手写递归
来源：http://gqh.hywenlv.cn

Go:   // 手写递归
来源：http://ljn.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iwh.c1oappe.top

C#:   // 手写递归
来源：http://wnd.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gqd.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xyb.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://thd.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://awr.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kka.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wfl.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ejw.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iyx.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bho.yj202588.top

================================================================================
来源：http://cjk.hesvh.cn

O. 并发与异步
来源：http://lyh.dianchejie.cn

================================================================================
来源：http://fza.xziqi.cn

[O01] 启动一个线程
来源：http://bqa.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://snn.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pqy.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mio.tarul.cn

TS:   // 同 JS
来源：http://sso.fktsv.cn

Java: new Thread(() -> f()).start()
来源：http://mqu.shuidangran.top

Go:   go f()
来源：http://ddo.zycfv.cn

Ruby: Thread.new { f }
来源：http://jar.epnwcf.com

C#:   Task.Run(() => F());
来源：http://hmj.ydzc1.top

[O02] 使用线程池
来源：http://xfe.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xtj.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qig.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://pcm.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://xhe.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sal.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lej.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wzh.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lvf.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://zpv.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://nia.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://vsi.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mha.cucudq.cn

TS:   // 同 JS
来源：http://zxq.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://xnj.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nxa.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vba.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://qru.ivvv.top

[O04] 定义异步函数并等待
来源：http://tee.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://avd.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qwb.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://wul.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qcw.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cdr.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qvt.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wyn.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://puf.hywenlv.cn

[O05] 并发执行并等待全部完成
来源：http://gxp.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://wlk.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ddf.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://pjh.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://goq.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jvc.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hcn.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://mtu.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nvr.daxiang520.top

[O06] 使用进程池
来源：http://ege.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yvj.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://efh.yonumen.top

JS:   // child_process / cluster 模块
来源：http://yjo.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://rig.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://grc.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://awr.uphjek.com

Ruby: // fork 块
来源：http://xik.dashuyun.cn

C#:   Parallel.For
来源：http://mnx.fehbvm.com

================================================================================
来源：http://jkt.52xcode.cn

P. 常用工具函数
来源：http://nwl.guannengcc.top

================================================================================
来源：http://kat.feifeiyinyue.top

[P01] 生成 UUID
来源：http://adl.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://rmo.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ijm.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://whj.iojbl.cn

TS:   crypto.randomUUID()
来源：http://whu.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://sgu.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://ilp.316326.xyz

Ruby: SecureRandom.uuid
来源：http://qyk.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://pqf.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://mxf.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xfm.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://swx.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kmz.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pfn.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wjr.yangfankeji.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vzp.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jko.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ypx.hnqzz.top

[P03] 生成短随机字符串
来源：http://rqn.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dzh.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rtv.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://chm.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://for.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bmm.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jvk.hcnkem.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ihw.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://smv.quarkkingdee.top

[P04] 求长度
来源：http://vuq.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lqe.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zaa.cqqwz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mkr.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://krf.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://ylp.sxryk.cn

Go:   len(arr);  len(m)
来源：http://lzs.fktsv.cn

Ruby: x.length;  x.size
来源：http://fwq.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://zzp.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://rxu.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tvi.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://poj.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jys.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jjc.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xfb.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vql.tianlin.xyz

Ruby: a == b
来源：http://qbi.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kwa.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kwz.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nrq.ivvv.top

PHP:  if (empty($x)) {}
来源：http://afz.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sno.sxryk.cn

TS:   if (x == null) {}
来源：http://yba.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bnc.guannengcc.top

Go:   if x == nil {}
来源：http://urf.haohaochexian.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://udi.zhongyouzk.top

C#:   if (x is null) {}
来源：http://qck.zhixingplan.top

[P07] 防抖与节流
来源：http://phw.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lom.havefunace.top

PHP:  // 手写时间戳比较
来源：http://nqb.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mrc.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twy.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wwh.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dgx.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://jzq.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vsm.yj20258.top

[P08] 处理浮点精度问题
来源：http://cjt.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zwm.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jwx.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oev.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jya.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hgx.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rwd.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zrg.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pdh.birdmap.top

================================================================================
来源：http://ouw.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://djx.meibo888.top

================================================================================
来源：http://hih.uphjek.com

[Q01] 创建表
来源：http://qxo.quarkkingdee.top

CREATE TABLE users (
来源：http://zey.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cef.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://zla.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://jmh.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ilh.yanxiufei.cn

);
来源：http://efg.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://lsf.sweek.top

CREATE TABLE orders (
来源：http://hsm.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tkr.gotoacloud.top

user_id INT NOT NULL,
来源：http://bxv.birdmap.top

amount DECIMAL(10, 2),
来源：http://vnw.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cfl.zycfv.cn

);
来源：http://xhp.zhengqikj.top

[Q03] 增加列
来源：http://twr.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lqh.vehdjk.com

[Q04] 修改列类型
来源：http://utc.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rwy.sysykeji.top

[Q05] 重命名列
来源：http://emk.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qcl.uphjek.com

[Q06] 删除列
来源：http://hyc.yj20258.top

ALTER TABLE users DROP COLUMN age;
来源：http://rur.cqqwz.cn

[Q07] 删除表
来源：http://ulu.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://bge.ivvv.top

[Q08] 创建普通索引
来源：http://ckv.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kod.smart0.xyz

[Q09] 创建唯一索引
来源：http://ryb.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lxu.yanxiufei.cn

[Q10] 插入单行
来源：http://umc.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jrf.iojbl.cn

[Q11] 一次插入多行
来源：http://yig.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zky.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://dqb.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://isy.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dvv.iojbl.cn

[Q13] 忽略重复插入
来源：http://fzb.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nvs.pengpengdd.cyou

[Q14] 存在则更新（upsert）
来源：http://yzc.tarul.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://syy.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://chu.hnxiangtu.top

[Q15] 查询全部
来源：http://una.shangyingyoupin.top

SELECT * FROM users;
来源：http://uhl.nwbrower.top

[Q16] 查询指定列
来源：http://crd.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://jhn.0kj1m.cn

[Q17] 条件查询
来源：http://wxj.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://slu.cheryme.top

[Q18] 模糊匹配
来源：http://xdf.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://div.uphjek.com

[Q19] 范围查询
来源：http://dvv.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pfh.bjfxy.top

[Q20] IN 列表
来源：http://ojh.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yhg.mhx1999.top

[Q21] 空值判断
来源：http://hfl.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kzl.hnqzz.top

[Q22] 排序
来源：http://nkn.iojbl.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qup.guowangkeji.top

[Q23] 分页
来源：http://etu.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gyc.xinyue.icu

[Q24] 去重
来源：http://tgq.yueranfly.top

SELECT DISTINCT city FROM users;
来源：http://hrz.gogol.net.cn

[Q25] 只取前 N 条
来源：http://esf.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zsp.yj20258.top

[Q26] 计数
来源：http://soa.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://ydk.redwolf501.top

[Q27] 条件计数
来源：http://yzh.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jnp.mhx1999.top

[Q28] 求和与平均
来源：http://jpa.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://omz.jinqigufen.top

[Q29] 最大最小值
来源：http://zla.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://rza.ivvv.top

[Q30] 分组统计
来源：http://zim.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kup.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://lrg.daxiang520.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ise.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://jde.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xad.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nfv.zhixingplan.top

[Q33] 多列分组
来源：http://nfl.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nup.ybcxt.top

[Q34] 每组取第一条
来源：http://rbc.gogol.net.cn

SELECT * FROM (
来源：http://nny.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iyk.fzhhl.top

) t WHERE rn = 1;
来源：http://ujx.gzhubu.top

[Q35] 内连接
来源：http://jez.zhengqikj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ssi.jinqigfzy.top

[Q36] 左连接
来源：http://way.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jsh.zycfv.cn

[Q37] 右连接
来源：http://nrn.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uxx.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://ywd.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ftn.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://ohr.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rad.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cin.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jrb.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bny.hnxiangtu.top

[Q41] 多表连接
来源：http://kki.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://zja.gogol.net.cn

JOIN users u ON u.id = o.user_id
来源：http://qdh.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://rgh.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://osf.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://gdi.gotoacloud.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xqw.zdqjudy.top

[Q43] 标量子查询
来源：http://uue.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qkq.ydjk.org.cn

[Q44] IN 子查询
来源：http://fyi.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zrz.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://kdk.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://efk.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://osr.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sgs.tian-w.cn

[Q47] 与平均值比较
来源：http://anl.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ywv.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://ffp.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hbl.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://tuu.chenjidiqi.icu

[Q49] 更新单行
来源：http://qhi.zhoulong.xyz


<!-- 参考信息 -->