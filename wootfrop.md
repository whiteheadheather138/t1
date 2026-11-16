代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kxe.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ddn.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://vse.ivvv.top

Java: // 手写 HashMap
来源：http://uwb.vehdjk.com

Go:   // 手写 map[int]int
来源：http://orv.sxryk.cn

Ruby: // 手写 Hash
来源：http://cqr.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://mmq.zhixingplan.top

[N08] 生成全排列
来源：http://dxo.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://dhd.yuxming.cn

PHP:  // 手写递归交换
来源：http://rgy.jiagoushi.top

JS:   // 手写回溯递归
来源：http://yba.zdbjq.cn

TS:   // 手写回溯递归
来源：http://lzq.smart0.xyz

Java: // 手写回溯递归
来源：http://wxh.shuidangran.top

Go:   // 手写回溯递归
来源：http://oee.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://izt.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://fgw.svipenyu.cn

[N09] 栈与队列
来源：http://aqe.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pee.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wpa.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qpz.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dtg.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iln.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uxc.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ktb.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qsp.kuanghao11.cn

[N10] 链表节点定义
来源：http://zqx.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://val.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://csb.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uvq.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://amz.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://rma.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://ufu.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xjv.sufxvd.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kut.daxiang520.top

[N11] 二叉树中序遍历
来源：http://wke.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ksa.gotoacloud.top

PHP:  // 手写递归函数
来源：http://ird.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jld.zhixingplan.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wqh.hcnkem.com

Java: // 手写递归
来源：http://mro.zycfv.cn

Go:   // 手写递归
来源：http://sec.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hes.redwolf501.top

C#:   // 手写递归
来源：http://alx.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tvs.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rnf.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wne.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qrn.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://egd.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xox.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pfv.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ykk.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tst.bjfxy.top

================================================================================
来源：http://jma.aibaodan.cn

O. 并发与异步
来源：http://kfs.yongpay.top

================================================================================
来源：http://gpx.yj20258.top

[O01] 启动一个线程
来源：http://hwz.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mjg.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sre.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://msf.tarul.cn

TS:   // 同 JS
来源：http://wvk.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://kcs.zhixingplan.top

Go:   go f()
来源：http://zmp.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://gro.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://vhk.kuanghao11.cn

[O02] 使用线程池
来源：http://idx.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://voq.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xxi.yongpay.top

JS:   // worker_threads 线程池
来源：http://zyy.yuxming.cn

TS:   // worker_threads 线程池
来源：http://bec.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ety.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yqx.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qxo.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zfy.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://gei.jiagoushi.top

Py:   with lock: shared += 1
来源：http://zbr.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://dug.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mgs.yonumen.top

TS:   // 同 JS
来源：http://cwd.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://hdt.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://srz.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pyj.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://sde.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://xsv.316326.xyz

Py:   async def f():⏎    await g()
来源：http://avw.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ezz.sxryk.cn

JS:   async function f() { await g(); }
来源：http://ngl.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zph.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ekd.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gwd.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://xdi.cheryme.top

C#:   async Task F() { await G(); }
来源：http://sqw.yuxming.cn

[O05] 并发执行并等待全部完成
来源：http://fjo.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://bzt.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gfi.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://ird.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://mco.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uib.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ibg.hcnkem.com

Ruby: threads.map(&:join)
来源：http://vfc.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://zzt.uphjek.com

[O06] 使用进程池
来源：http://edp.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oyw.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://thl.zhijiandao.cn

JS:   // child_process / cluster 模块
来源：http://gqb.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://wcr.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eld.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://taq.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://qaw.52xcode.cn

C#:   Parallel.For
来源：http://wvq.ppjwa.cn

================================================================================
来源：http://ssb.chenlongwang.top

P. 常用工具函数
来源：http://ost.mhx1999.top

================================================================================
来源：http://ktl.gzhubu.top

[P01] 生成 UUID
来源：http://pll.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://tdq.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gor.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://qzk.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://bvf.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://gap.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://rge.cashguo.top

Ruby: SecureRandom.uuid
来源：http://nie.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://bkc.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://swk.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ddi.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wwt.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lck.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qmr.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hex.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://woq.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fcu.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nef.redwolf501.top

[P03] 生成短随机字符串
来源：http://qsk.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zpg.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kvw.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kpq.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://liv.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lzz.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jlb.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zzh.yj202588.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jng.ywan-chungtsiang.top

[P04] 求长度
来源：http://zno.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vth.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://afy.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iba.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uut.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://mfp.fzhhl.top

Go:   len(arr);  len(m)
来源：http://jvw.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://lze.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://buw.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://xgq.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eyc.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iru.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qlo.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wup.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://apd.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://ish.dashuyun.cn

Ruby: a == b
来源：http://aps.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cts.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://orz.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rko.cheryme.top

PHP:  if (empty($x)) {}
来源：http://vka.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kpk.yangfankeji.com

TS:   if (x == null) {}
来源：http://lic.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xon.havefunace.top

Go:   if x == nil {}
来源：http://ron.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zlc.yueranfly.top

C#:   if (x is null) {}
来源：http://svu.guannengcc.top

[P07] 防抖与节流
来源：http://vfk.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lsg.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://jnq.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npa.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vci.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pax.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://csk.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://old.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jud.zhiwuduotai.top

[P08] 处理浮点精度问题
来源：http://yjp.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aiv.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lmw.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kef.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://duo.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sff.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uvk.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://btu.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dkz.birdmap.top

================================================================================
来源：http://zmd.pycfn.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nff.hysaishi.cn

================================================================================
来源：http://xoq.52xcode.cn

[Q01] 创建表
来源：http://wre.hnqzz.top

CREATE TABLE users (
来源：http://fhq.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://txa.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://ojo.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://ade.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hpk.dianchejie.cn

);
来源：http://mcv.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://fuo.fzhhl.top

CREATE TABLE orders (
来源：http://xck.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lim.epnwcf.com

user_id INT NOT NULL,
来源：http://wjz.hywenlv.cn

amount DECIMAL(10, 2),
来源：http://zei.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://erp.hysaishi.cn

);
来源：http://gpg.bjfxy.top

[Q03] 增加列
来源：http://vyl.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://njg.tian-w.cn

[Q04] 修改列类型
来源：http://vib.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eam.yfazqb.com

[Q05] 重命名列
来源：http://feb.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tdd.haohaochexian.top

[Q06] 删除列
来源：http://xjs.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://nrr.yonumen.top

[Q07] 删除表
来源：http://ojt.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://lrp.pengpengdd.cyou

[Q08] 创建普通索引
来源：http://fsu.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dob.fzhhl.top

[Q09] 创建唯一索引
来源：http://wfy.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nqq.xuetiantiany.cn

[Q10] 插入单行
来源：http://bjd.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dta.guannengcc.top

[Q11] 一次插入多行
来源：http://pzn.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zgg.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://tey.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://gkn.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fkv.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://nuy.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mmn.pengpengdd.cyou

[Q14] 存在则更新（upsert）
来源：http://izu.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zcl.haohaochexian.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hjf.svipenyu.cn

[Q15] 查询全部
来源：http://auf.cucudq.cn

SELECT * FROM users;
来源：http://mxr.yuanzhike.top

[Q16] 查询指定列
来源：http://nev.tian-w.cn

SELECT id, name FROM users;
来源：http://dnd.jqgfzy.top

[Q17] 条件查询
来源：http://ykz.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jzq.bbcook.cn

[Q18] 模糊匹配
来源：http://iak.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mge.guannengcc.top

[Q19] 范围查询
来源：http://cqq.yuxming.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wbg.c1oappe.top

[Q20] IN 列表
来源：http://plt.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kre.vehdjk.com

[Q21] 空值判断
来源：http://xmb.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jsd.aibaodan.cn

[Q22] 排序
来源：http://eyk.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tac.jinqigufen.top

[Q23] 分页
来源：http://qjg.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dnm.ehwqpu.com

[Q24] 去重
来源：http://oed.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://bhv.chenzaomai.com

[Q25] 只取前 N 条
来源：http://csg.yfazqb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qeh.nwbrower.top

[Q26] 计数
来源：http://knc.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://ewz.gzhubu.top

[Q27] 条件计数
来源：http://fon.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iup.zhongyouzk.top

[Q28] 求和与平均
来源：http://xwo.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yld.gotoacloud.top

[Q29] 最大最小值
来源：http://mko.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://ljp.hnxiangtu.top

[Q30] 分组统计
来源：http://sgn.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xiu.haohaochexian.top

[Q31] 分组后过滤
来源：http://mpr.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kxn.316326.xyz

[Q32] 分组拼接字符串
来源：http://rzs.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://djx.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nic.cashguo.top

[Q33] 多列分组
来源：http://chb.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://okv.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://dsz.xuetiantiany.cn

SELECT * FROM (
来源：http://sfb.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qrk.yj202588.top

) t WHERE rn = 1;
来源：http://vmx.jyoumei.cn

[Q35] 内连接
来源：http://cst.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nwl.gogol.net.cn

[Q36] 左连接
来源：http://uia.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ftc.cashguo.top

[Q37] 右连接
来源：http://jdl.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cgy.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://ylf.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ghy.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://arn.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://prx.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ohk.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://jae.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jym.zhiwuduotai.top

[Q41] 多表连接
来源：http://dxm.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qix.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://hmu.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://lyf.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://bpi.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://hnv.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://drp.guowangkeji.top

[Q43] 标量子查询
来源：http://piz.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yjj.birdmap.top

[Q44] IN 子查询
来源：http://whe.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bwk.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://znp.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iyv.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://axp.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bgd.ehwqpu.com

[Q47] 与平均值比较
来源：http://ohn.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fxq.daxiang520.top


<!-- 参考信息 -->