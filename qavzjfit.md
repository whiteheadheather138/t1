代发 wailian999

Ruby: s == s.reverse
来源：http://pnm.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://huz.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://lbd.havefunace.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ahq.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mtl.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ckd.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://vxo.yfazqb.com

Java: // 手写 HashMap
来源：http://mfc.hcnkem.com

Go:   // 手写 map[int]int
来源：http://not.zhengqikj.top

Ruby: // 手写 Hash
来源：http://pxr.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://ykj.dashuyun.cn

[N08] 生成全排列
来源：http://bap.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://yky.ctjpmb.com

PHP:  // 手写递归交换
来源：http://jkf.fktsv.cn

JS:   // 手写回溯递归
来源：http://yfo.xylfe.cn

TS:   // 手写回溯递归
来源：http://xtb.dashuyun.cn

Java: // 手写回溯递归
来源：http://gjh.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://wnh.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://szf.jiagoushi.top

C#:   // 手写回溯递归
来源：http://azh.c1oappe.top

[N09] 栈与队列
来源：http://alb.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://abs.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tza.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://maa.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://llm.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fxt.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ohb.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kbx.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dtl.zdqjudy.top

[N10] 链表节点定义
来源：http://zap.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rzm.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://agy.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xco.yangfankeji.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tbc.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://gub.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://wwh.vqdsnc.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gtp.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mls.xylfe.cn

[N11] 二叉树中序遍历
来源：http://toz.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kly.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://wwh.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lsn.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xnz.nanxuanxn.top

Java: // 手写递归
来源：http://tnk.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://fpu.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ebq.xinyue.icu

C#:   // 手写递归
来源：http://owe.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hef.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cze.hywenlv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xiy.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wov.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sur.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wlz.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://scc.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dwq.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qyz.vehdjk.com

================================================================================
来源：http://elb.hcnkem.com

O. 并发与异步
来源：http://uiz.daria6918.cn

================================================================================
来源：http://rip.zhixingplan.top

[O01] 启动一个线程
来源：http://mft.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vit.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://txe.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ceb.dashuyun.cn

TS:   // 同 JS
来源：http://qbw.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://sft.yuanzhike.top

Go:   go f()
来源：http://zrb.vehdjk.com

Ruby: Thread.new { f }
来源：http://kyy.birdmap.top

C#:   Task.Run(() => F());
来源：http://hyw.yvedp.cn

[O02] 使用线程池
来源：http://gpr.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rvb.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qvh.yongpay.top

JS:   // worker_threads 线程池
来源：http://sus.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://vcc.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://uyi.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sro.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wut.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xeg.uphjek.com

[O03] 加锁保护共享数据
来源：http://uuo.iojbl.cn

Py:   with lock: shared += 1
来源：http://dhs.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://mzz.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jmp.ydjk.org.cn

TS:   // 同 JS
来源：http://leh.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://gcr.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hlc.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mmn.zdqjudy.top

C#:   lock (gate) { shared++; }
来源：http://ufq.xziqi.cn

[O04] 定义异步函数并等待
来源：http://jum.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://bqt.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gca.xuanzx.com

JS:   async function f() { await g(); }
来源：http://ydf.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://frs.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tuy.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aws.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://mve.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://clo.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://wye.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://fmo.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fbv.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://sht.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://euw.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://crt.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://anq.yfazqb.com

Ruby: threads.map(&:join)
来源：http://exf.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hjj.vehdjk.com

[O06] 使用进程池
来源：http://oqg.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cxh.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jjy.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://lkn.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://iko.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rsz.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tpl.hcnkem.com

Ruby: // fork 块
来源：http://mff.tianlin.xyz

C#:   Parallel.For
来源：http://tvn.tianlin.xyz

================================================================================
来源：http://odm.shzxlz.cn

P. 常用工具函数
来源：http://uck.ppjwa.cn

================================================================================
来源：http://myt.gotoacloud.top

[P01] 生成 UUID
来源：http://cub.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://rry.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jah.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://zgq.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://pqf.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://amx.0kj1m.cn

Go:   // 用 github.com/google/uuid
来源：http://cdt.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://qun.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://gee.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://gvr.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://swh.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pcr.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xqu.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ljq.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ozk.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tes.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://twb.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hem.cheryme.top

[P03] 生成短随机字符串
来源：http://vmh.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zrn.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zzg.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://szw.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://znn.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qil.mhx1999.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eof.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jbf.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hci.yuanzhike.top

[P04] 求长度
来源：http://ljz.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gtr.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://skq.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fau.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://brx.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://xtv.yonumen.top

Go:   len(arr);  len(m)
来源：http://nyz.mhx1999.top

Ruby: x.length;  x.size
来源：http://mmd.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hmy.yanxiufei.cn

[P05] 判断两个对象内容是否相等
来源：http://ytw.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fwz.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rog.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://msr.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rvo.sweek.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yjk.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ztp.zhijiandao.cn

Ruby: a == b
来源：http://yjg.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ona.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qfz.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qfv.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://bxw.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ltb.cucudq.cn

TS:   if (x == null) {}
来源：http://pbf.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lkk.zhijiandao.cn

Go:   if x == nil {}
来源：http://wlk.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nxh.cucudq.cn

C#:   if (x is null) {}
来源：http://rgl.hesvh.cn

[P07] 防抖与节流
来源：http://ryc.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kzu.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://zse.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://arn.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dnf.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aar.jqgufenzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tnl.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dvh.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dzl.jqgfzy.top

[P08] 处理浮点精度问题
来源：http://hha.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lbr.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://url.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lwv.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ush.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zqd.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sej.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yva.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vjt.c1oappe.top

================================================================================
来源：http://fko.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hdn.ivvv.top

================================================================================
来源：http://sju.gotoacloud.top

[Q01] 创建表
来源：http://zik.yuanzhike.top

CREATE TABLE users (
来源：http://akl.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tkw.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://wof.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://jvl.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://duw.smart0.xyz

);
来源：http://hjx.yfazqb.com

[Q02] 创建带外键的表
来源：http://rzu.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://ogr.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://djq.yj202588.top

user_id INT NOT NULL,
来源：http://wnr.yonumen.top

amount DECIMAL(10, 2),
来源：http://cwr.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tix.hnqzz.top

);
来源：http://mkc.sufxvd.cn

[Q03] 增加列
来源：http://utr.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://frh.yuanzhike.top

[Q04] 修改列类型
来源：http://avr.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://won.jqgfzy.top

[Q05] 重命名列
来源：http://nrs.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mbh.fehbvm.com

[Q06] 删除列
来源：http://wyy.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cpw.iojbl.cn

[Q07] 删除表
来源：http://xty.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://kij.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://kwl.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xcr.ctjpmb.com

[Q09] 创建唯一索引
来源：http://tim.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kek.yuanzhike.top

[Q10] 插入单行
来源：http://jkm.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ycn.zhongyouzk.top

[Q11] 一次插入多行
来源：http://sgg.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cvy.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://bsy.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://woo.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tvt.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://ete.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wtk.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://kfw.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nlh.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://amw.gotoacloud.top

[Q15] 查询全部
来源：http://bvw.hcnkem.com

SELECT * FROM users;
来源：http://lub.zhengqikj.top

[Q16] 查询指定列
来源：http://jeq.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://kof.zhaomingkeji.xyz

[Q17] 条件查询
来源：http://mjq.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://top.nanxuanxn.top

[Q18] 模糊匹配
来源：http://bre.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iwv.yueranfly.top

[Q19] 范围查询
来源：http://yvp.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xse.cdnleiting.top

[Q20] IN 列表
来源：http://mlx.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ybc.zdbjq.cn

[Q21] 空值判断
来源：http://knm.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://wxt.zdbjq.cn

[Q22] 排序
来源：http://mnd.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uci.gaohongyu789.top

[Q23] 分页
来源：http://czo.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ewq.yj20258888.top

[Q24] 去重
来源：http://piw.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://gnm.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://rok.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://trs.nanxuanxn.top

[Q26] 计数
来源：http://egh.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://jgr.9152youxi.cn

[Q27] 条件计数
来源：http://vhl.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vpg.svipenyu.cn

[Q28] 求和与平均
来源：http://fku.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kro.fktsv.cn

[Q29] 最大最小值
来源：http://mla.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sfc.gotoacloud.top

[Q30] 分组统计
来源：http://nve.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ust.cqqwz.cn

[Q31] 分组后过滤
来源：http://ijq.daxiang520.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ucd.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://ttn.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://myq.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kzc.xinyue.icu

[Q33] 多列分组
来源：http://seq.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gcx.aizwys.cn

[Q34] 每组取第一条
来源：http://yta.gzhubu.top

SELECT * FROM (
来源：http://bdx.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ack.hesvh.cn

) t WHERE rn = 1;
来源：http://jtw.chenjidiqi.icu

[Q35] 内连接
来源：http://mhc.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://unl.ppjwa.cn

[Q36] 左连接
来源：http://crd.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dey.gaohongyu789.top

[Q37] 右连接
来源：http://jvp.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uxh.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://ang.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ytb.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://gbg.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qdp.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wan.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nti.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gjt.chenzaomai.com

[Q41] 多表连接
来源：http://vqz.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ytu.yvedp.cn

JOIN users u ON u.id = o.user_id
来源：http://nib.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://gbt.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://wmn.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://ymz.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fjx.vehdjk.com

[Q43] 标量子查询
来源：http://qwc.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ala.zhoulong.xyz

[Q44] IN 子查询
来源：http://cda.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nry.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://zfx.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ajn.zdqjudy.top


<!-- 参考信息 -->