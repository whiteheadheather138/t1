代发 wailian999

Ruby: s == s.reverse
来源：http://fhg.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://rhe.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://mrs.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cty.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uje.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lsq.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://acl.dashuyun.cn

Java: // 手写 HashMap
来源：http://ket.jianghu66.top

Go:   // 手写 map[int]int
来源：http://zhl.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://blq.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wqq.jianghu66.top

[N08] 生成全排列
来源：http://akc.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://wpu.yfazqb.com

PHP:  // 手写递归交换
来源：http://lkx.ivvv.top

JS:   // 手写回溯递归
来源：http://ahm.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://cbq.zhijiandao.cn

Java: // 手写回溯递归
来源：http://ogf.yj20258888.top

Go:   // 手写回溯递归
来源：http://ged.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://ggy.fengsongda.top

C#:   // 手写回溯递归
来源：http://nfm.jqgufenzy.top

[N09] 栈与队列
来源：http://yud.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://srl.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wls.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wsr.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mhz.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jku.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jvu.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wfg.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jnq.zdbjq.cn

[N10] 链表节点定义
来源：http://qxr.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ldl.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yhv.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ycl.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mhr.birdmap.top

Java: class Node { int v; Node next; }
来源：http://rpc.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://vzy.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gkr.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qom.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://quc.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wxu.bjfxy.top

PHP:  // 手写递归函数
来源：http://nui.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://edy.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://atk.ivvv.top

Java: // 手写递归
来源：http://cho.hesvh.cn

Go:   // 手写递归
来源：http://pmd.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bhn.hysaishi.cn

C#:   // 手写递归
来源：http://ehu.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yjd.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jnk.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zlg.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yre.hywenlv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cmm.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rau.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vcb.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dan.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ifk.pycfn.com

================================================================================
来源：http://eqd.shanyushiyangtech.top

O. 并发与异步
来源：http://pmk.yongpay.top

================================================================================
来源：http://wfa.jyoumei.cn

[O01] 启动一个线程
来源：http://hmy.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dzi.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eft.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sas.pycfn.com

TS:   // 同 JS
来源：http://vjq.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://epy.smart0.xyz

Go:   go f()
来源：http://hst.birdmap.top

Ruby: Thread.new { f }
来源：http://hgt.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://cmw.hfpthk.cn

[O02] 使用线程池
来源：http://jje.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cxb.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qkx.epnwcf.com

JS:   // worker_threads 线程池
来源：http://ptv.andypj.xyz

TS:   // worker_threads 线程池
来源：http://ify.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://prf.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pza.birdmap.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pem.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oqm.hammf.cn

[O03] 加锁保护共享数据
来源：http://klu.yvedp.cn

Py:   with lock: shared += 1
来源：http://tba.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://ktp.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tqy.bbcook.cn

TS:   // 同 JS
来源：http://mqp.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://znv.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bih.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tzk.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://tlf.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://qzt.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://fcr.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://njz.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://bqk.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yzn.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lbu.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ysh.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xkm.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://brr.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://ncq.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://yye.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hzj.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://uck.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://psq.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vul.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ptz.hammf.cn

Ruby: threads.map(&:join)
来源：http://uml.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lrz.ydzc1.top

[O06] 使用进程池
来源：http://xzh.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://unb.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://hej.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://crv.uphjek.com

TS:   // child_process / cluster 模块
来源：http://lbw.gaohongyu789.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jho.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xji.iojbl.cn

Ruby: // fork 块
来源：http://iby.birdmap.top

C#:   Parallel.For
来源：http://wpe.fzhhl.top

================================================================================
来源：http://oud.epnwcf.com

P. 常用工具函数
来源：http://oqg.yueranfly.top

================================================================================
来源：http://zwj.yj20258.top

[P01] 生成 UUID
来源：http://cph.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://ntj.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oot.hongshengwenyu.top

JS:   crypto.randomUUID()
来源：http://uhn.yvedp.cn

TS:   crypto.randomUUID()
来源：http://drb.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://flm.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://ywg.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://oyt.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://kjn.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://mpb.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ada.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://piy.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wjs.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lsj.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vmt.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://amv.tianlin.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qyq.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://npw.fengsongda.top

[P03] 生成短随机字符串
来源：http://rnu.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tas.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ssp.ybcxt.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yma.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rsy.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ldv.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ixq.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lfu.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vwk.sxryk.cn

[P04] 求长度
来源：http://lfe.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jcb.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oai.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bbm.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fpu.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://klj.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://ggz.ivvv.top

Ruby: x.length;  x.size
来源：http://gdc.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rym.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://isb.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://tkd.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dyi.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jhy.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zhj.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mvu.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yfd.svipenyu.cn

Ruby: a == b
来源：http://bgs.uphjek.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vsk.jinqigufen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yxz.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fif.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://ndx.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bya.tianlin.xyz

TS:   if (x == null) {}
来源：http://jsl.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ews.ppjwa.cn

Go:   if x == nil {}
来源：http://jid.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iyj.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://wyo.shzxlz.cn

[P07] 防抖与节流
来源：http://ogd.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pjz.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://tdk.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://buz.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hqw.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jjw.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pav.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://avr.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://thq.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://rbv.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bvw.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://exo.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://idt.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://odm.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zgt.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://naw.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pul.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qtv.jqgufenzy.top

================================================================================
来源：http://xyx.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mlm.fktsv.cn

================================================================================
来源：http://gdp.mhx1999.top

[Q01] 创建表
来源：http://wnp.hysaishi.cn

CREATE TABLE users (
来源：http://fis.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aet.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://bww.daria6918.cn

email VARCHAR(100) UNIQUE,
来源：http://wfz.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lap.zhaomingkeji.xyz

);
来源：http://osn.ybcxt.top

[Q02] 创建带外键的表
来源：http://wpl.zhongyouzk.top

CREATE TABLE orders (
来源：http://mvx.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hky.ydzc1.top

user_id INT NOT NULL,
来源：http://ofg.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://imo.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tku.smart0.xyz

);
来源：http://qnq.quarkkingdee.top

[Q03] 增加列
来源：http://nws.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ycm.ydzc1.top

[Q04] 修改列类型
来源：http://xrl.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ixo.shzxlz.cn

[Q05] 重命名列
来源：http://lvx.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rcq.sjlbkw.cn

[Q06] 删除列
来源：http://kpi.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://lli.316326.xyz

[Q07] 删除表
来源：http://pwm.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://tja.vqdsnc.cn

[Q08] 创建普通索引
来源：http://rcu.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fzd.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://gxd.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jpg.zhoulong.xyz

[Q10] 插入单行
来源：http://bjn.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://byr.yangfankeji.com

[Q11] 一次插入多行
来源：http://uyb.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sni.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://zfg.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://hom.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yen.daxiang520.top

[Q13] 忽略重复插入
来源：http://apl.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kld.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://vye.yangfankeji.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://akc.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ffd.shangyingyoupin.top

[Q15] 查询全部
来源：http://pbk.quarkkingdee.top

SELECT * FROM users;
来源：http://guz.jinqigfzy.top

[Q16] 查询指定列
来源：http://wts.aibaodan.cn

SELECT id, name FROM users;
来源：http://xua.jyoumei.cn

[Q17] 条件查询
来源：http://zbz.gogol.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gqt.hysaishi.cn

[Q18] 模糊匹配
来源：http://rrb.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://stn.cheryme.top

[Q19] 范围查询
来源：http://hit.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bxn.redwolf501.top

[Q20] IN 列表
来源：http://mzk.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wtf.xuetiantiany.cn

[Q21] 空值判断
来源：http://ylz.hysaishi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://klm.gaohongyu789.top

[Q22] 排序
来源：http://daz.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pzu.zdqjudy.top

[Q23] 分页
来源：http://daq.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ruc.c1oappe.top

[Q24] 去重
来源：http://lec.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://cwx.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://ycw.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://thj.aibaodan.cn

[Q26] 计数
来源：http://mjp.xinyue.icu

SELECT COUNT(*) FROM users;
来源：http://kgy.xziqi.cn

[Q27] 条件计数
来源：http://foi.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dfc.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://ufn.jqgufenzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://irm.yuxming.cn

[Q29] 最大最小值
来源：http://ivb.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vsc.hysaishi.cn

[Q30] 分组统计
来源：http://fko.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oqb.iojbl.cn

[Q31] 分组后过滤
来源：http://sfz.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qzv.xziqi.cn

[Q32] 分组拼接字符串
来源：http://fji.yonumen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oez.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ftz.smart0.xyz

[Q33] 多列分组
来源：http://eep.andypj.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pas.daria6918.cn

[Q34] 每组取第一条
来源：http://yhv.jqgfzy.top

SELECT * FROM (
来源：http://tzb.52xcode.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fyt.redwolf501.top

) t WHERE rn = 1;
来源：http://rby.snrcjt.cn

[Q35] 内连接
来源：http://etk.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://egx.shzxlz.cn

[Q36] 左连接
来源：http://wgo.0kj1m.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://opp.gaohongyu789.top

[Q37] 右连接
来源：http://tva.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cyg.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://psd.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hhp.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://zhm.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rjn.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dkk.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ssi.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mkb.jiagoushi.top

[Q41] 多表连接
来源：http://duy.dianchejie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wjm.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://ylo.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://ara.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://oqj.tian-w.cn

SELECT u.name, o.amount FROM users u
来源：http://drb.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jzr.wangshuangyany.cn

[Q43] 标量子查询
来源：http://lgf.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yqt.cdnleiting.top

[Q44] IN 子查询
来源：http://vdw.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ahh.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://ppy.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rft.jqgufenzy.top


<!-- 参考信息 -->