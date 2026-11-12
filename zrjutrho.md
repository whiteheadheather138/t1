代发 wailian999

Py:   itertools.permutations(arr)
来源：http://rur.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://gok.hysaishi.cn

JS:   // 手写回溯递归
来源：http://ldz.yueranfly.top

TS:   // 手写回溯递归
来源：http://ohp.gaohongyu789.top

Java: // 手写回溯递归
来源：http://gxq.uphjek.com

Go:   // 手写回溯递归
来源：http://hbe.uphjek.com

Ruby: arr.permutation.to_a
来源：http://inq.shuidangran.top

C#:   // 手写回溯递归
来源：http://ihm.fktsv.cn

[N09] 栈与队列
来源：http://rhq.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oyy.wangdashe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kyv.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vrq.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zsx.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fbv.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iqq.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ijk.chenjidiqi.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nmi.hywenlv.cn

[N10] 链表节点定义
来源：http://ere.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mir.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rnu.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fmk.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kso.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://fna.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://ody.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://adb.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://tap.cashguo.top

[N11] 二叉树中序遍历
来源：http://kuo.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pff.yueranfly.top

PHP:  // 手写递归函数
来源：http://xsi.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ocy.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tvt.dianchejie.cn

Java: // 手写递归
来源：http://abk.wangdashe.top

Go:   // 手写递归
来源：http://zzn.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://azo.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://xlf.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pbf.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vsn.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qbp.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugs.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://knd.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hyg.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://axm.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ddh.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xwj.mhx1999.top

================================================================================
来源：http://kfk.yongpay.top

O. 并发与异步
来源：http://yxz.tianlin.xyz

================================================================================
来源：http://mqg.zhijiandao.cn

[O01] 启动一个线程
来源：http://twg.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qtb.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zwj.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ahn.yangfankeji.com

TS:   // 同 JS
来源：http://yak.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://tpn.cdnleiting.top

Go:   go f()
来源：http://fdd.yangfankeji.com

Ruby: Thread.new { f }
来源：http://sjt.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://pkc.redwolf501.top

[O02] 使用线程池
来源：http://ajn.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mks.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vht.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://thz.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://rpn.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eot.cdnleiting.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xws.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aep.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yql.wangshuangyany.cn

[O03] 加锁保护共享数据
来源：http://qco.daria6918.cn

Py:   with lock: shared += 1
来源：http://uuc.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://swd.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oxk.hammf.cn

TS:   // 同 JS
来源：http://oka.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://fkd.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wxp.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hrm.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://egz.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://wyx.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://kgv.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gom.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://nrk.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zfm.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bal.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uhk.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://roz.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://vpq.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://xos.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://kia.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wst.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://epo.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://lry.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vtl.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gkt.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://dzv.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://hep.ybcxt.top

[O06] 使用进程池
来源：http://omf.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ehz.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://faq.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://wga.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://bgw.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zsw.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hnj.pengpengdd.cyou

Ruby: // fork 块
来源：http://rtg.wangshuangyany.cn

C#:   Parallel.For
来源：http://dwk.mhx1999.top

================================================================================
来源：http://cie.svipenyu.cn

P. 常用工具函数
来源：http://xhj.vehdjk.com

================================================================================
来源：http://udr.havefunace.top

[P01] 生成 UUID
来源：http://efr.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://rfz.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gdm.nwbrower.top

JS:   crypto.randomUUID()
来源：http://ayq.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://ubt.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://yff.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://vws.pycfn.com

Ruby: SecureRandom.uuid
来源：http://kjn.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://wqk.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://kce.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ypb.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lmo.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://scg.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ifq.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sdf.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tox.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zdv.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wcn.nanxinkj.top

[P03] 生成短随机字符串
来源：http://gpx.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bxk.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rjy.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vyr.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kum.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rpz.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hsu.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vrx.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vrz.cashguo.top

[P04] 求长度
来源：http://siw.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vjj.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://woj.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://egl.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yrb.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://drp.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://ons.c1oappe.top

Ruby: x.length;  x.size
来源：http://aox.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ebb.tianlin.xyz

[P05] 判断两个对象内容是否相等
来源：http://eok.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bij.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vvy.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uos.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://elp.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jus.shanyushiyangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://cej.hesvh.cn

Ruby: a == b
来源：http://ach.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pkr.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lma.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ejs.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://njn.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dyu.cheryme.top

TS:   if (x == null) {}
来源：http://jsf.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mst.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://hrl.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qvd.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://fjj.316326.xyz

[P07] 防抖与节流
来源：http://trf.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hnn.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://wsg.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zex.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hfd.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ucz.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nvs.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hmx.ywan-chungtsiang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dgz.vehdjk.com

[P08] 处理浮点精度问题
来源：http://nxd.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wbb.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qia.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zyx.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wqw.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nqy.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wiz.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ysv.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zvg.yuxming.cn

================================================================================
来源：http://aws.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qsl.dashuyun.cn

================================================================================
来源：http://xft.sxryk.cn

[Q01] 创建表
来源：http://yje.pengpengdd.cyou

CREATE TABLE users (
来源：http://kdv.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qif.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://igu.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://vbw.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://egh.vehdjk.com

);
来源：http://jpn.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://bmt.feifeiyinyue.top

CREATE TABLE orders (
来源：http://ksf.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fdj.yanxiufei.cn

user_id INT NOT NULL,
来源：http://nvg.meibo888.top

amount DECIMAL(10, 2),
来源：http://zoi.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sro.ctjpmb.com

);
来源：http://xai.xylfe.cn

[Q03] 增加列
来源：http://ckw.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vnb.chenzaomai.com

[Q04] 修改列类型
来源：http://vpd.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gqw.nanxuanxn.top

[Q05] 重命名列
来源：http://vwt.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mem.jinghuilouyu.cn

[Q06] 删除列
来源：http://rnz.havefunace.top

ALTER TABLE users DROP COLUMN age;
来源：http://trp.zhengqikj.top

[Q07] 删除表
来源：http://mah.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://efs.ydjk.org.cn

[Q08] 创建普通索引
来源：http://ozt.haohaochexian.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mom.hysaishi.cn

[Q09] 创建唯一索引
来源：http://dpq.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ivp.fengsongda.top

[Q10] 插入单行
来源：http://gmn.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mqa.yonumen.top

[Q11] 一次插入多行
来源：http://jgw.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://clu.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://kqf.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://pjb.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qpw.hnqzz.top

[Q13] 忽略重复插入
来源：http://ytp.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rsq.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://kzw.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bnj.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wzl.zhixingplan.top

[Q15] 查询全部
来源：http://oor.zhongyouzk.top

SELECT * FROM users;
来源：http://coj.jinqigfzy.top

[Q16] 查询指定列
来源：http://aac.ehwqpu.com

SELECT id, name FROM users;
来源：http://aby.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://tks.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hub.ydzc1.top

[Q18] 模糊匹配
来源：http://ryy.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wst.wangshuangyany.cn

[Q19] 范围查询
来源：http://iec.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zdx.mhx1999.top

[Q20] IN 列表
来源：http://vup.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lzw.cdnleiting.top

[Q21] 空值判断
来源：http://uan.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xlq.shuidangran.top

[Q22] 排序
来源：http://cxi.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nze.c1oappe.top

[Q23] 分页
来源：http://aro.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tib.gogol.net.cn

[Q24] 去重
来源：http://mri.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://hsm.hammf.cn

[Q25] 只取前 N 条
来源：http://ycj.cucudq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://phj.ybcxt.top

[Q26] 计数
来源：http://lsa.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://gwc.wangdashe.top

[Q27] 条件计数
来源：http://nuf.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oqa.cqqwz.cn

[Q28] 求和与平均
来源：http://mne.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://woo.gzhubu.top

[Q29] 最大最小值
来源：http://wfp.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vxy.daxiang520.top

[Q30] 分组统计
来源：http://xdy.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cbp.haohaochexian.top

[Q31] 分组后过滤
来源：http://sav.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uoy.hesvh.cn

[Q32] 分组拼接字符串
来源：http://nfx.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bvq.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://exx.xinyue.icu

[Q33] 多列分组
来源：http://njv.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lon.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://kkn.bjfxy.top

SELECT * FROM (
来源：http://rtt.jyoumei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pgw.quarkkingdee.top

) t WHERE rn = 1;
来源：http://quv.hnxiangtu.top

[Q35] 内连接
来源：http://dlt.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pez.yueranfly.top

[Q36] 左连接
来源：http://lhs.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zwo.aizwys.cn

[Q37] 右连接
来源：http://dxx.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lob.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://sep.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wgx.meibo888.top

[Q39] 自连接（查上下级）
来源：http://oof.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dij.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dtg.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pwj.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fuh.jinghuilouyu.cn

[Q41] 多表连接
来源：http://kdv.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://tfi.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://qnf.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://ndk.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://nrf.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://nhy.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wvd.gotoacloud.top

[Q43] 标量子查询
来源：http://jed.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zie.ppjwa.cn

[Q44] IN 子查询
来源：http://wuz.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yqw.yj202588.top

[Q45] EXISTS 判断存在
来源：http://rbw.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dpx.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://miu.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fus.xziqi.cn

[Q47] 与平均值比较
来源：http://pje.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://osn.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://jrk.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qfy.fengsongda.top

SELECT * FROM t WHERE c > 5;
来源：http://eda.zdbjq.cn

[Q49] 更新单行
来源：http://mqq.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rcj.wangdashe.top

[Q50] 批量更新
来源：http://wgh.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jti.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://ing.zdbjq.cn


<!-- 参考信息 -->