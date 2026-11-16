代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zpq.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pxj.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://ztv.9152youxi.cn

Java: // 手写 HashMap
来源：http://wfb.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://lix.chenlongwang.top

Ruby: // 手写 Hash
来源：http://qoo.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eyc.52xcode.cn

[N08] 生成全排列
来源：http://fpg.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://nek.aizwys.cn

PHP:  // 手写递归交换
来源：http://olj.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://uqo.smart0.xyz

TS:   // 手写回溯递归
来源：http://znd.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://ktu.jianghu66.top

Go:   // 手写回溯递归
来源：http://nvf.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://lbm.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://exh.bjfxy.top

[N09] 栈与队列
来源：http://ihy.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eyu.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://adj.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pkf.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://omj.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://liw.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://irx.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dvd.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mzs.ydjk.org.cn

[N10] 链表节点定义
来源：http://ihw.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hzm.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mpl.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nab.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gdn.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://xuu.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://mip.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://amy.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://etj.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://wsv.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ajz.andypj.xyz

PHP:  // 手写递归函数
来源：http://fan.zhixingplan.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mcr.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rog.pycfn.com

Java: // 手写递归
来源：http://dvp.ppjwa.cn

Go:   // 手写递归
来源：http://joo.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xsi.ydjk.org.cn

C#:   // 手写递归
来源：http://hoi.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vpi.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cpg.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tbr.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esy.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wag.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lui.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bze.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fzg.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ppf.chenlongwang.top

================================================================================
来源：http://owi.daxiang520.top

O. 并发与异步
来源：http://lwm.hfpthk.cn

================================================================================
来源：http://opm.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://qis.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yce.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wcf.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gwj.snrcjt.cn

TS:   // 同 JS
来源：http://dxf.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://xng.zhoulong.xyz

Go:   go f()
来源：http://llo.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://uld.smart0.xyz

C#:   Task.Run(() => F());
来源：http://sjj.hammf.cn

[O02] 使用线程池
来源：http://ijb.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pcc.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nrb.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://yfv.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://qiy.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://bsp.cucudq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fws.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://htc.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vtq.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://asb.ppjwa.cn

Py:   with lock: shared += 1
来源：http://kkh.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://wuy.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aaz.hesvh.cn

TS:   // 同 JS
来源：http://yvy.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://aru.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ynf.vqdsnc.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://udd.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://wjv.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://tyf.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://xtx.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mfu.316326.xyz

JS:   async function f() { await g(); }
来源：http://peb.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://uxs.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tlt.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vme.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://tfk.tian-w.cn

C#:   async Task F() { await G(); }
来源：http://xag.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://vxr.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://via.pengpengdd.cyou

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lzj.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://nhw.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://qwh.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pxt.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hpr.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://zke.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ozm.shzxlz.cn

[O06] 使用进程池
来源：http://zff.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bxq.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ymh.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://mgy.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://zca.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ole.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lxk.0kj1m.cn

Ruby: // fork 块
来源：http://xhr.snrcjt.cn

C#:   Parallel.For
来源：http://ckm.shanyushiyangtech.top

================================================================================
来源：http://vnj.hnxiangtu.top

P. 常用工具函数
来源：http://pku.yj20258.top

================================================================================
来源：http://cgp.sufxvd.cn

[P01] 生成 UUID
来源：http://iie.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://vch.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yvk.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://fse.yfazqb.com

TS:   crypto.randomUUID()
来源：http://abi.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://dzl.nanxinkj.top

Go:   // 用 github.com/google/uuid
来源：http://ecu.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://tsp.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://xxm.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://bnm.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wul.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dxh.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sre.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bkg.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vjb.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://did.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kyy.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://llr.yuanzhike.top

[P03] 生成短随机字符串
来源：http://kqz.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mvd.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dxg.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lyt.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zbd.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://shj.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tsw.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cef.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hkx.jinqigfzy.top

[P04] 求长度
来源：http://ftc.nwbrower.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ylv.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bdv.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://okg.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgs.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://wju.bbcook.cn

Go:   len(arr);  len(m)
来源：http://hlm.nwbrower.top

Ruby: x.length;  x.size
来源：http://blf.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wwj.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://uuu.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://czs.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xzc.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xxn.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lzz.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eov.zdqjudy.top

Go:   reflect.DeepEqual(a, b)
来源：http://mse.zhoulong.xyz

Ruby: a == b
来源：http://tpr.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gnu.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gvn.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hjn.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://eqm.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cgn.hysaishi.cn

TS:   if (x == null) {}
来源：http://hux.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wof.pycfn.com

Go:   if x == nil {}
来源：http://lcy.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://znh.jianghu66.top

C#:   if (x is null) {}
来源：http://cmf.cdnleiting.top

[P07] 防抖与节流
来源：http://efz.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hgm.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://nru.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zmc.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://leh.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://viq.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hml.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://btv.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rfa.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://vgy.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ltg.zdqjudy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://arx.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aai.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kbf.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hun.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://orz.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jih.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lqu.yfazqb.com

================================================================================
来源：http://tpa.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xlg.gzhubu.top

================================================================================
来源：http://pbg.jinqigufen.top

[Q01] 创建表
来源：http://kha.zhoulong.xyz

CREATE TABLE users (
来源：http://ryu.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rki.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://smg.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://dhy.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://omy.yanxiufei.cn

);
来源：http://rqe.hcnkem.com

[Q02] 创建带外键的表
来源：http://smv.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://dkg.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vnc.tian-w.cn

user_id INT NOT NULL,
来源：http://fox.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://wal.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aah.feifeiyinyue.top

);
来源：http://ftj.yj202588.top

[Q03] 增加列
来源：http://ylg.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cey.yangfankeji.com

[Q04] 修改列类型
来源：http://ker.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gqm.ehwqpu.com

[Q05] 重命名列
来源：http://vbw.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xph.dianchejie.cn

[Q06] 删除列
来源：http://nvo.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://gip.cdnleiting.top

[Q07] 删除表
来源：http://ywo.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://ufp.yj20258888.top

[Q08] 创建普通索引
来源：http://rxl.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xtd.daria6918.cn

[Q09] 创建唯一索引
来源：http://jaz.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://flt.cqqwz.cn

[Q10] 插入单行
来源：http://egu.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cno.zdqjudy.top

[Q11] 一次插入多行
来源：http://hlg.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lws.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://mcc.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://cin.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lsf.dianchejie.cn

[Q13] 忽略重复插入
来源：http://zis.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pzi.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://zzn.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dpk.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mef.yueranfly.top

[Q15] 查询全部
来源：http://cls.yonumen.top

SELECT * FROM users;
来源：http://jhj.smart0.xyz

[Q16] 查询指定列
来源：http://oxr.sysykeji.top

SELECT id, name FROM users;
来源：http://koh.jiagoushi.top

[Q17] 条件查询
来源：http://coc.aibaodan.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pyy.ivvv.top

[Q18] 模糊匹配
来源：http://djt.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://faq.yuanzhike.top

[Q19] 范围查询
来源：http://kjn.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kgd.shzxlz.cn

[Q20] IN 列表
来源：http://vvr.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ssc.cucudq.cn

[Q21] 空值判断
来源：http://ldt.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ogz.epnwcf.com

[Q22] 排序
来源：http://evf.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nqa.jinghuilouyu.cn

[Q23] 分页
来源：http://tvc.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ddc.nwbrower.top

[Q24] 去重
来源：http://mfm.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://yfq.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://oww.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kwb.cdnleiting.top

[Q26] 计数
来源：http://qoz.dianchejie.cn

SELECT COUNT(*) FROM users;
来源：http://ryv.0kj1m.cn

[Q27] 条件计数
来源：http://egv.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pif.316326.xyz

[Q28] 求和与平均
来源：http://swy.aibaodan.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dxu.9152youxi.cn

[Q29] 最大最小值
来源：http://cly.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cmb.andypj.xyz

[Q30] 分组统计
来源：http://tdx.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xrq.sjlbkw.cn

[Q31] 分组后过滤
来源：http://oaz.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://swa.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://ysu.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zal.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bln.hywenlv.cn

[Q33] 多列分组
来源：http://wgj.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cee.vehdjk.com

[Q34] 每组取第一条
来源：http://tug.nwbrower.top

SELECT * FROM (
来源：http://rcd.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pek.hysaishi.cn

) t WHERE rn = 1;
来源：http://hfp.ppjwa.cn

[Q35] 内连接
来源：http://kmz.zhiwuduotai.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sle.zhongyouzk.top

[Q36] 左连接
来源：http://lvv.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qep.hysaishi.cn

[Q37] 右连接
来源：http://qbd.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vwg.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://stq.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jyz.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://hok.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tbb.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fqy.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://odg.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://avr.havefunace.top

[Q41] 多表连接
来源：http://jjm.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vwt.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://aqn.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://vnu.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://xzz.0kj1m.cn

SELECT u.name, o.amount FROM users u
来源：http://unu.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qid.wangshuangyany.cn

[Q43] 标量子查询
来源：http://zfs.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hzz.vehdjk.com

[Q44] IN 子查询
来源：http://ivx.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zsl.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://rmk.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cuu.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://ysj.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mrl.0kj1m.cn

[Q47] 与平均值比较
来源：http://sbt.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://veo.fengsongda.top


<!-- 参考信息 -->