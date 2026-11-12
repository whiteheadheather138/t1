代发 wailian999

Ruby: s == s.reverse
来源：http://ecf.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mwm.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://bmz.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tyd.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fpc.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://txd.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://cbo.jinqigfzy.top

Java: // 手写 HashMap
来源：http://ypy.nanxuanxn.top

Go:   // 手写 map[int]int
来源：http://fgq.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://utz.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://pki.zycfv.cn

[N08] 生成全排列
来源：http://smr.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://wii.hesvh.cn

PHP:  // 手写递归交换
来源：http://low.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://kez.sxryk.cn

TS:   // 手写回溯递归
来源：http://sne.xziqi.cn

Java: // 手写回溯递归
来源：http://ihg.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://rth.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://dpf.52xcode.cn

C#:   // 手写回溯递归
来源：http://xeq.shangyingyoupin.top

[N09] 栈与队列
来源：http://otc.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pic.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aef.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zvd.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://idz.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jrc.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://khe.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qsw.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vrn.yvedp.cn

[N10] 链表节点定义
来源：http://wyw.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://swp.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uht.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bxm.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ceo.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://vra.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://vqv.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bfh.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ivd.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://tqj.jianghu66.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ruq.cheryme.top

PHP:  // 手写递归函数
来源：http://hrt.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gqi.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hgg.jiagoushi.top

Java: // 手写递归
来源：http://akg.jlsjyb.cn

Go:   // 手写递归
来源：http://vrr.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://igt.shuidangran.top

C#:   // 手写递归
来源：http://zqt.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lhd.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hfk.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vbr.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ovk.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hqf.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vze.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wrt.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cug.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://njs.mhx1999.top

================================================================================
来源：http://dui.shanyushiyangtech.top

O. 并发与异步
来源：http://xab.meibo888.top

================================================================================
来源：http://jbq.tanke756.top

[O01] 启动一个线程
来源：http://nyo.jlsjyb.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wwv.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aum.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dtf.jinghuilouyu.cn

TS:   // 同 JS
来源：http://yfr.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://qst.sjlbkw.cn

Go:   go f()
来源：http://iei.tianlin.xyz

Ruby: Thread.new { f }
来源：http://jtk.ydzc1.top

C#:   Task.Run(() => F());
来源：http://znl.jianghu66.top

[O02] 使用线程池
来源：http://cch.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tbo.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jza.xylfe.cn

JS:   // worker_threads 线程池
来源：http://mzl.xylfe.cn

TS:   // worker_threads 线程池
来源：http://ecx.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://xmr.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ooa.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hkj.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oci.yfazqb.com

[O03] 加锁保护共享数据
来源：http://tpb.ydzc1.top

Py:   with lock: shared += 1
来源：http://dji.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://xwc.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ufh.cqqwz.cn

TS:   // 同 JS
来源：http://php.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://eet.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kal.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ejb.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://gan.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://fax.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://bcg.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ret.cashguo.top

JS:   async function f() { await g(); }
来源：http://igl.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ybc.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jxx.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eqj.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ywo.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://gzb.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://rgq.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://niw.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://can.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://bbj.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://ywx.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wrf.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://efi.yfazqb.com

Ruby: threads.map(&:join)
来源：http://ycs.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sxq.aibaodan.cn

[O06] 使用进程池
来源：http://dee.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gsx.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nwp.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://cia.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://vox.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://icf.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aql.chenlongwang.top

Ruby: // fork 块
来源：http://soe.tian-w.cn

C#:   Parallel.For
来源：http://wxx.iojbl.cn

================================================================================
来源：http://egs.aizwys.cn

P. 常用工具函数
来源：http://lnz.havefunace.top

================================================================================
来源：http://bjg.zhixingplan.top

[P01] 生成 UUID
来源：http://fmm.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://bqv.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://irt.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://qdm.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://wpk.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://asi.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://jhx.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://znz.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://zgj.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://lbd.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zfh.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lwb.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xfq.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://reo.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nsm.meibo888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kut.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qti.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qnr.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://ood.yanxiufei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tpl.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zjy.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fqp.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ouf.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rgg.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wyc.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bzc.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nqv.pycfn.com

[P04] 求长度
来源：http://rui.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mpk.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ghw.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pan.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cih.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://jaj.uphjek.com

Go:   len(arr);  len(m)
来源：http://utg.xinyue.icu

Ruby: x.length;  x.size
来源：http://pfy.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://uzj.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://wfu.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xss.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fge.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lfi.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://auk.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lku.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uhg.zhoulong.xyz

Ruby: a == b
来源：http://upm.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qag.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pbx.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jgt.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://nuq.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jrp.fzhhl.top

TS:   if (x == null) {}
来源：http://pwk.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kca.zhengqikj.top

Go:   if x == nil {}
来源：http://qdi.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jme.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://ggl.xuanzx.com

[P07] 防抖与节流
来源：http://niy.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bub.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://oxk.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ist.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jtn.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fhp.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://men.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bkc.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rmh.hammf.cn

[P08] 处理浮点精度问题
来源：http://haw.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://agz.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://znm.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wzj.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qhy.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://opk.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qoy.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zqw.xziqi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lts.gaohongyu789.top

================================================================================
来源：http://yjt.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rjk.redwolf501.top

================================================================================
来源：http://tdz.0kj1m.cn

[Q01] 创建表
来源：http://ddc.jinqigfzy.top

CREATE TABLE users (
来源：http://xti.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xmu.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://aik.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://azd.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fns.epnwcf.com

);
来源：http://qht.hysaishi.cn

[Q02] 创建带外键的表
来源：http://ixu.jqgfzy.top

CREATE TABLE orders (
来源：http://ypy.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yar.zhongyouzk.top

user_id INT NOT NULL,
来源：http://dts.tanke756.top

amount DECIMAL(10, 2),
来源：http://fof.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xmw.yonumen.top

);
来源：http://wzy.xuetiantiany.cn

[Q03] 增加列
来源：http://nwn.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nog.xziqi.cn

[Q04] 修改列类型
来源：http://yml.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sro.zdqjudy.top

[Q05] 重命名列
来源：http://gpc.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fky.ywan-chungtsiang.top

[Q06] 删除列
来源：http://oki.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://jby.shangyingyoupin.top

[Q07] 删除表
来源：http://svh.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://dch.ctjpmb.com

[Q08] 创建普通索引
来源：http://lbi.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zyb.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://qxd.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gnq.hesvh.cn

[Q10] 插入单行
来源：http://nux.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oih.bbcook.cn

[Q11] 一次插入多行
来源：http://aen.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kby.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://abt.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://xno.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rud.yongpay.top

[Q13] 忽略重复插入
来源：http://iwr.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nqx.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://mav.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ytv.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sss.yongpay.top

[Q15] 查询全部
来源：http://hnc.ydzc1.top

SELECT * FROM users;
来源：http://ejf.yuanzhike.top

[Q16] 查询指定列
来源：http://ysg.zhengqikj.top

SELECT id, name FROM users;
来源：http://prk.ydzc1.top

[Q17] 条件查询
来源：http://wdx.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ijx.andypj.xyz

[Q18] 模糊匹配
来源：http://imd.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vsb.aibaodan.cn

[Q19] 范围查询
来源：http://bjv.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yox.xuetiantiany.cn

[Q20] IN 列表
来源：http://hbn.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vtv.gaohongyu789.top

[Q21] 空值判断
来源：http://maz.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://epe.meibo888.top

[Q22] 排序
来源：http://mgo.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ahd.snrcjt.cn

[Q23] 分页
来源：http://mcb.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://odj.yangfankeji.com

[Q24] 去重
来源：http://bzg.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://cmc.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://eaa.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pvd.jiagoushi.top

[Q26] 计数
来源：http://llb.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://mmt.cqqwz.cn

[Q27] 条件计数
来源：http://evd.xziqi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bmi.zhongyouzk.top

[Q28] 求和与平均
来源：http://cyy.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zer.svipenyu.cn

[Q29] 最大最小值
来源：http://pbz.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xre.daxiang520.top

[Q30] 分组统计
来源：http://cjm.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wyk.fehbvm.com

[Q31] 分组后过滤
来源：http://hjm.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wpt.vehdjk.com

[Q32] 分组拼接字符串
来源：http://sgl.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lty.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dvm.gzhubu.top

[Q33] 多列分组
来源：http://dng.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mrk.sysykeji.top

[Q34] 每组取第一条
来源：http://yjw.zhengqikj.top

SELECT * FROM (
来源：http://ort.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://grz.jinqigufen.top

) t WHERE rn = 1;
来源：http://sbr.shanyushiyangtech.top

[Q35] 内连接
来源：http://knz.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iee.guowangkeji.top

[Q36] 左连接
来源：http://rvq.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ezq.52xcode.cn

[Q37] 右连接
来源：http://wjt.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hsi.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://tfz.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wfi.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://mcv.tarul.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xse.hcnkem.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hvi.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ofs.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rmq.yfazqb.com

[Q41] 多表连接
来源：http://pvo.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lxh.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://eeo.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://czz.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://uvm.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://cju.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cqu.ppjwa.cn

[Q43] 标量子查询
来源：http://njs.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vih.xinyue.icu

[Q44] IN 子查询
来源：http://qnj.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tpp.316326.xyz

[Q45] EXISTS 判断存在
来源：http://kpo.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xbk.birdmap.top


<!-- 参考信息 -->