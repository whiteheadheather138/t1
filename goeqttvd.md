代发 wailian999

Java: // 手写回溯递归
来源：http://wvd.fehbvm.com

Go:   // 手写回溯递归
来源：http://fwn.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://owi.xylfe.cn

C#:   // 手写回溯递归
来源：http://dzp.vehdjk.com

[N09] 栈与队列
来源：http://rmx.daria6918.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pti.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jdz.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fyt.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bfz.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pxt.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bys.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mix.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kpd.yangfankeji.com

[N10] 链表节点定义
来源：http://fku.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://unk.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://brn.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fyk.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ate.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://ttl.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://llc.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xqi.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uvi.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://ubk.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ngu.xziqi.cn

PHP:  // 手写递归函数
来源：http://nqw.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rkp.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yzk.hysaishi.cn

Java: // 手写递归
来源：http://gta.smart0.xyz

Go:   // 手写递归
来源：http://hdt.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://epz.ctjpmb.com

C#:   // 手写递归
来源：http://crt.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xrc.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iby.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fqm.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gpj.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://imj.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kgg.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nue.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bzb.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xad.yvedp.cn

================================================================================
来源：http://kct.xuanzx.com

O. 并发与异步
来源：http://ycf.zdqjudy.top

================================================================================
来源：http://qmw.wangdashe.top

[O01] 启动一个线程
来源：http://ees.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ajz.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gug.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://txa.jinqigufen.top

TS:   // 同 JS
来源：http://ert.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://kvr.zhongyouzk.top

Go:   go f()
来源：http://znf.ivvv.top

Ruby: Thread.new { f }
来源：http://kos.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://lra.yuxming.cn

[O02] 使用线程池
来源：http://cua.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eqc.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mqc.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://ema.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://wnz.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://ynv.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://myr.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://epf.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bgb.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://weq.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://hzm.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://nmk.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eqw.birdmap.top

TS:   // 同 JS
来源：http://xli.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://ssu.iojbl.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hxb.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tab.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://eed.havefunace.top

[O04] 定义异步函数并等待
来源：http://qyh.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://zxy.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ijc.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://ngs.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://csd.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uyd.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oqx.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://dvz.xinyue.icu

C#:   async Task F() { await G(); }
来源：http://phl.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://kjj.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://tsl.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zza.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://ofv.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://dyc.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://byq.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://crx.fehbvm.com

Ruby: threads.map(&:join)
来源：http://sen.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jyo.sweek.top

[O06] 使用进程池
来源：http://trm.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vgc.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kpp.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://mgq.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://bzl.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qwm.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mio.jlsjyb.cn

Ruby: // fork 块
来源：http://wnq.yongpay.top

C#:   Parallel.For
来源：http://daf.quarkkingdee.top

================================================================================
来源：http://gdx.kuanghao11.cn

P. 常用工具函数
来源：http://fqi.shanyushiyangtech.top

================================================================================
来源：http://zyk.xziqi.cn

[P01] 生成 UUID
来源：http://ysb.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://kav.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://plv.cucudq.cn

JS:   crypto.randomUUID()
来源：http://qnt.c1oappe.top

TS:   crypto.randomUUID()
来源：http://zaa.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://gsg.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://crk.hammf.cn

Ruby: SecureRandom.uuid
来源：http://sno.xingfuxueyuan.xyz

C#:   Guid.NewGuid().ToString()
来源：http://jtp.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://sxd.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wdv.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vmd.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://skl.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gql.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jkt.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://idz.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fvx.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zqo.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://ghf.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://npk.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dds.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hsw.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cyd.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mzi.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://psq.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mul.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://paw.yj202588.top

[P04] 求长度
来源：http://rxm.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xef.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lkp.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pcq.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kia.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://uks.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://vyc.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://xzz.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://wdo.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://luc.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zvy.tianlin.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pbp.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://epu.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wxc.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mbi.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://wka.sysykeji.top

Ruby: a == b
来源：http://dvm.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ebr.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xff.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dxv.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://dtk.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bje.smart0.xyz

TS:   if (x == null) {}
来源：http://igv.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vff.jinqigfzy.top

Go:   if x == nil {}
来源：http://kkw.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xrg.xinyue.icu

C#:   if (x is null) {}
来源：http://rkd.quarkkingdee.top

[P07] 防抖与节流
来源：http://fbd.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vqc.cashguo.top

PHP:  // 手写时间戳比较
来源：http://gwv.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pux.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bjm.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tqx.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gxr.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bvf.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xml.hcnkem.com

[P08] 处理浮点精度问题
来源：http://bkq.9152youxi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nbt.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jph.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uip.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jvq.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gfa.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hrq.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bqk.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qff.jinyuanbaomall.cn

================================================================================
来源：http://yoi.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zur.ehwqpu.com

================================================================================
来源：http://cpv.jinyuanbaomall.cn

[Q01] 创建表
来源：http://vgy.hnqzz.top

CREATE TABLE users (
来源：http://dfg.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fqy.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://rbx.sysykeji.top

email VARCHAR(100) UNIQUE,
来源：http://wyp.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://epy.hcnkem.com

);
来源：http://aya.fktsv.cn

[Q02] 创建带外键的表
来源：http://atw.xinyue.icu

CREATE TABLE orders (
来源：http://tte.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://atj.vehdjk.com

user_id INT NOT NULL,
来源：http://vhq.ydzc1.top

amount DECIMAL(10, 2),
来源：http://vka.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://frz.andypj.xyz

);
来源：http://fmc.feifeiyinyue.top

[Q03] 增加列
来源：http://ghy.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fui.gzhubu.top

[Q04] 修改列类型
来源：http://mkk.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mvc.gotoacloud.top

[Q05] 重命名列
来源：http://eio.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mty.iojbl.cn

[Q06] 删除列
来源：http://equ.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vgv.ctjpmb.com

[Q07] 删除表
来源：http://lkt.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://tfx.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://xxv.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hrg.epnwcf.com

[Q09] 创建唯一索引
来源：http://met.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kvb.shuidangran.top

[Q10] 插入单行
来源：http://teg.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wjk.cucudq.cn

[Q11] 一次插入多行
来源：http://wbi.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cqq.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://lkc.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ycm.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rdv.chenlongwang.top

[Q13] 忽略重复插入
来源：http://hoj.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kly.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://xqx.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kks.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ktp.guannengcc.top

[Q15] 查询全部
来源：http://smq.jyoumei.cn

SELECT * FROM users;
来源：http://whh.0kj1m.cn

[Q16] 查询指定列
来源：http://uwf.jqgufenzy.top

SELECT id, name FROM users;
来源：http://wrn.zdbjq.cn

[Q17] 条件查询
来源：http://fdk.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aus.jiagoushi.top

[Q18] 模糊匹配
来源：http://bok.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jaz.cucudq.cn

[Q19] 范围查询
来源：http://liq.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hnb.yongpay.top

[Q20] IN 列表
来源：http://zse.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oov.nanxinkj.top

[Q21] 空值判断
来源：http://jfg.hysaishi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bov.zdbjq.cn

[Q22] 排序
来源：http://rbq.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dbn.shanyushiyangtech.top

[Q23] 分页
来源：http://cxi.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wbn.ybcxt.top

[Q24] 去重
来源：http://hgc.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://rhw.vehdjk.com

[Q25] 只取前 N 条
来源：http://soh.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fgx.zycfv.cn

[Q26] 计数
来源：http://jyv.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://xlm.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://owl.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zai.jianghu66.top

[Q28] 求和与平均
来源：http://fie.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wth.svipenyu.cn

[Q29] 最大最小值
来源：http://uks.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lxr.zhoulong.xyz

[Q30] 分组统计
来源：http://ipi.sxryk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://okr.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://sok.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qhp.yj202588.top

[Q32] 分组拼接字符串
来源：http://fei.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qxw.yangfankeji.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rmt.jinqigfzy.top

[Q33] 多列分组
来源：http://uva.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://frd.yueranfly.top

[Q34] 每组取第一条
来源：http://pby.ctjpmb.com

SELECT * FROM (
来源：http://isg.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://psf.fehbvm.com

) t WHERE rn = 1;
来源：http://inb.dianchejie.cn

[Q35] 内连接
来源：http://khr.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fbh.haohaochexian.top

[Q36] 左连接
来源：http://kwm.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gqx.chenzaomai.com

[Q37] 右连接
来源：http://ess.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tql.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xnv.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hvp.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://xof.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rnm.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mhi.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xjq.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://apm.zhoulong.xyz

[Q41] 多表连接
来源：http://zth.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://zjn.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://syg.haohaochexian.top

JOIN products p ON p.id = o.product_id;
来源：http://idv.52xcode.cn

[Q42] 连接条件附加过滤
来源：http://mna.mhx1999.top

SELECT u.name, o.amount FROM users u
来源：http://joc.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://taz.snrcjt.cn

[Q43] 标量子查询
来源：http://afv.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vlk.aibaodan.cn

[Q44] IN 子查询
来源：http://owa.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bsy.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://pdz.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fge.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://edc.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://avj.redwolf501.top

[Q47] 与平均值比较
来源：http://ynx.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://epe.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://pii.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fdl.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://qnt.zhixingplan.top

[Q49] 更新单行
来源：http://ney.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yhh.wangdashe.top

[Q50] 批量更新
来源：http://fja.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hcc.wangdashe.top

[Q51] 用子查询更新
来源：http://ucb.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nbi.dashuyun.cn

[Q52] 删除指定行
来源：http://zad.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://fer.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://ddr.daxiang520.top


<!-- 参考信息 -->