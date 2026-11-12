代发 wailian999

Java: // 手写回溯递归
来源：http://zrc.jiagoushi.top

Go:   // 手写回溯递归
来源：http://pcv.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://kan.smart0.xyz

C#:   // 手写回溯递归
来源：http://iyy.jinghuilouyu.cn

[N09] 栈与队列
来源：http://gss.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xwm.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bnu.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vvk.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fca.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://net.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fxl.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fkz.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ujy.hongshengwenyu.top

[N10] 链表节点定义
来源：http://lhd.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dhe.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://clu.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://duj.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://quv.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://gqx.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://adq.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://unv.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nmp.daria6918.cn

[N11] 二叉树中序遍历
来源：http://aug.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kkx.smart0.xyz

PHP:  // 手写递归函数
来源：http://zeb.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xez.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bmv.jyoumei.cn

Java: // 手写递归
来源：http://yuj.fehbvm.com

Go:   // 手写递归
来源：http://dqm.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vah.bjfxy.top

C#:   // 手写递归
来源：http://hrg.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eii.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yii.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fvm.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qyg.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oxx.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ygo.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dng.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jwh.hnqzz.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qtw.tian-w.cn

================================================================================
来源：http://uqk.xylfe.cn

O. 并发与异步
来源：http://suf.cheryme.top

================================================================================
来源：http://rhm.shangyingyoupin.top

[O01] 启动一个线程
来源：http://jcl.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eqq.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pvg.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jqr.hysaishi.cn

TS:   // 同 JS
来源：http://bcu.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://cve.nanxuanxn.top

Go:   go f()
来源：http://svt.daria6918.cn

Ruby: Thread.new { f }
来源：http://ltm.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://hym.ywan-chungtsiang.top

[O02] 使用线程池
来源：http://dmz.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pet.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hzw.tianlin.xyz

JS:   // worker_threads 线程池
来源：http://nuw.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://xua.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://xev.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jmj.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iuw.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wgw.tian-w.cn

[O03] 加锁保护共享数据
来源：http://joi.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://yte.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://lll.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lte.yongpay.top

TS:   // 同 JS
来源：http://btk.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://dly.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pzt.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rws.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://egs.zycfv.cn

[O04] 定义异步函数并等待
来源：http://bsv.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://hkj.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://twk.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://ojk.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://qmz.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://afz.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://edr.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://cie.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://aaa.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://vti.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://cwj.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oza.tarul.cn

JS:   await Promise.all(tasks)
来源：http://aba.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://msk.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ktt.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rja.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://mhh.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ecz.hfpthk.cn

[O06] 使用进程池
来源：http://pat.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://akt.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://avi.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://vcd.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://kkz.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lad.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dwa.fehbvm.com

Ruby: // fork 块
来源：http://bro.mhx1999.top

C#:   Parallel.For
来源：http://wop.fanxiaobao.xyz

================================================================================
来源：http://qso.zhongyouzk.top

P. 常用工具函数
来源：http://txk.ctjpmb.com

================================================================================
来源：http://ybt.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://evn.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://uvm.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ggo.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://xru.aizwys.cn

TS:   crypto.randomUUID()
来源：http://wwc.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://wqj.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://kir.jinyuanbaomall.cn

Ruby: SecureRandom.uuid
来源：http://imo.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://onn.52xcode.cn

[P02] MD5 / SHA256 摘要
来源：http://lsc.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lcz.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://not.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lag.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wiy.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rnd.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oog.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ghs.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eqg.sweek.top

[P03] 生成短随机字符串
来源：http://fsn.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://utk.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nhb.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zfs.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lld.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ytv.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wsz.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://foc.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zkt.gogol.net.cn

[P04] 求长度
来源：http://ady.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cly.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://epx.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lqn.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://axk.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://gsh.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://cqa.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://uxe.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cgz.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://lfe.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rrz.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hbp.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mwf.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tud.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cxw.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vkm.zhoulong.xyz

Ruby: a == b
来源：http://tse.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://udz.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wjm.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eng.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://lmz.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://opi.ybcxt.top

TS:   if (x == null) {}
来源：http://uau.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yoz.kuanghao11.cn

Go:   if x == nil {}
来源：http://pcu.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dnv.hnxiangtu.top

C#:   if (x is null) {}
来源：http://dsb.52xcode.cn

[P07] 防抖与节流
来源：http://cmo.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://utp.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://nbu.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wbo.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://plj.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cfr.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uso.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://frl.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cow.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://dil.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wfn.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lhd.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uwj.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zdd.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://imr.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gjp.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ads.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jsx.jinyuanbaomall.cn

================================================================================
来源：http://wvl.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uad.havefunace.top

================================================================================
来源：http://uhm.9152youxi.cn

[Q01] 创建表
来源：http://xdq.vqdsnc.cn

CREATE TABLE users (
来源：http://sdw.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hbd.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://kjz.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://dda.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rsa.daxiang520.top

);
来源：http://frl.aibaodan.cn

[Q02] 创建带外键的表
来源：http://nrw.zdbjq.cn

CREATE TABLE orders (
来源：http://faq.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yze.zdbjq.cn

user_id INT NOT NULL,
来源：http://ppr.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://xkt.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dgz.daria6918.cn

);
来源：http://qrj.shuidangran.top

[Q03] 增加列
来源：http://dle.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bar.hywenlv.cn

[Q04] 修改列类型
来源：http://lnf.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xvt.zhengqikj.top

[Q05] 重命名列
来源：http://gfj.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://feg.cdnleiting.top

[Q06] 删除列
来源：http://ltn.ctjpmb.com

ALTER TABLE users DROP COLUMN age;
来源：http://uei.shangyingyoupin.top

[Q07] 删除表
来源：http://uwb.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://xwl.yj20258888.top

[Q08] 创建普通索引
来源：http://fkd.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://bzu.snrcjt.cn

[Q09] 创建唯一索引
来源：http://unh.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wyp.fanxiaobao.xyz

[Q10] 插入单行
来源：http://toe.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ytv.nanxinkj.top

[Q11] 一次插入多行
来源：http://kcw.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://duw.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://vmu.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lim.zhoulong.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kdy.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://eyo.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rjq.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://lze.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://emc.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vue.cheryme.top

[Q15] 查询全部
来源：http://lhs.hesvh.cn

SELECT * FROM users;
来源：http://mxs.nanxuanxn.top

[Q16] 查询指定列
来源：http://xlo.gogol.net.cn

SELECT id, name FROM users;
来源：http://bwt.daxiang520.top

[Q17] 条件查询
来源：http://nbu.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bzk.birdmap.top

[Q18] 模糊匹配
来源：http://mmv.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jyg.sysykeji.top

[Q19] 范围查询
来源：http://ehc.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aky.gogol.net.cn

[Q20] IN 列表
来源：http://oot.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qxs.redwolf501.top

[Q21] 空值判断
来源：http://lqu.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://zpi.tian-w.cn

[Q22] 排序
来源：http://zhl.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gii.tanke756.top

[Q23] 分页
来源：http://ksv.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fpv.0kj1m.cn

[Q24] 去重
来源：http://vng.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://hpu.jqgfzy.top

[Q25] 只取前 N 条
来源：http://ijy.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pvj.shanyushiyangkeji.top

[Q26] 计数
来源：http://mkh.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://pvd.zdqjudy.top

[Q27] 条件计数
来源：http://gam.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zew.yj20258888.top

[Q28] 求和与平均
来源：http://sxe.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lsl.sxryk.cn

[Q29] 最大最小值
来源：http://uns.jyoumei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jzy.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://syp.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mdw.yuxming.cn

[Q31] 分组后过滤
来源：http://omy.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sif.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://ylv.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hcj.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wnz.hfpthk.cn

[Q33] 多列分组
来源：http://abe.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lcf.yongpay.top

[Q34] 每组取第一条
来源：http://wcc.fanxiaobao.xyz

SELECT * FROM (
来源：http://tlc.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bgk.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://hvp.jqgufenzy.top

[Q35] 内连接
来源：http://gjc.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tqe.vehdjk.com

[Q36] 左连接
来源：http://gjl.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kla.ppjwa.cn

[Q37] 右连接
来源：http://ocu.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jwp.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://upj.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vnr.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://wqb.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vcu.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tcm.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wad.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ksc.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://bfz.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yde.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://syr.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://ykq.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://aqq.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://hjn.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xfo.chenzaomai.com

[Q43] 标量子查询
来源：http://oup.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zqq.zhixingplan.top

[Q44] IN 子查询
来源：http://nvd.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ivo.pycfn.com

[Q45] EXISTS 判断存在
来源：http://hzk.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://unt.mhx1999.top

[Q46] NOT EXISTS 判断不存在
来源：http://vba.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lyf.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://jth.svipenyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rsm.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://rtm.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gms.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://hva.52xcode.cn

[Q49] 更新单行
来源：http://zlu.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rgu.yj20258888.top

[Q50] 批量更新
来源：http://eoh.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://les.yonumen.top

[Q51] 用子查询更新
来源：http://cmp.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qxo.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://rmx.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://xxr.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://dcj.chenjidiqi.icu


<!-- 参考信息 -->