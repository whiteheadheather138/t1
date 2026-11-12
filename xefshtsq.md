代发 wailian999

Java: // 手写回溯递归
来源：http://fzw.nwbrower.top

Go:   // 手写回溯递归
来源：http://ygh.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://ozu.hammf.cn

C#:   // 手写回溯递归
来源：http://vvr.c1oappe.top

[N09] 栈与队列
来源：http://awi.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oev.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lcu.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jcs.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dvi.xylfe.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rci.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ixw.jiagoushi.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cjd.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://svc.hysaishi.cn

[N10] 链表节点定义
来源：http://rnk.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rmh.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://ctk.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://phm.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dvh.tanke756.top

Java: class Node { int v; Node next; }
来源：http://zyb.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fsg.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tds.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nsv.fktsv.cn

[N11] 二叉树中序遍历
来源：http://eeg.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zud.yonumen.top

PHP:  // 手写递归函数
来源：http://wte.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fle.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlr.cheryme.top

Java: // 手写递归
来源：http://bqp.redwolf501.top

Go:   // 手写递归
来源：http://kcg.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pls.hammf.cn

C#:   // 手写递归
来源：http://cvg.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ggs.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hgo.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qxa.fengsongda.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tqk.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hsm.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qwy.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lxx.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sph.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wmy.cqqwz.cn

================================================================================
来源：http://pqw.yueranfly.top

O. 并发与异步
来源：http://ery.bjfxy.top

================================================================================
来源：http://sdw.c1oappe.top

[O01] 启动一个线程
来源：http://tdq.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gwq.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pfy.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bzj.andypj.xyz

TS:   // 同 JS
来源：http://yed.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://phq.guannengcc.top

Go:   go f()
来源：http://rdo.0kj1m.cn

Ruby: Thread.new { f }
来源：http://xso.iojbl.cn

C#:   Task.Run(() => F());
来源：http://euy.ydjk.org.cn

[O02] 使用线程池
来源：http://mmx.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://epn.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dyc.xziqi.cn

JS:   // worker_threads 线程池
来源：http://oou.yj20258888.top

TS:   // worker_threads 线程池
来源：http://ajw.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://rfn.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ozf.fktsv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rjq.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hro.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://hws.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://kwz.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://nhl.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xjq.ivvv.top

TS:   // 同 JS
来源：http://nrn.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://meq.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ycm.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dbn.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://dqr.316326.xyz

[O04] 定义异步函数并等待
来源：http://apu.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://ckl.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kuz.yfazqb.com

JS:   async function f() { await g(); }
来源：http://jsn.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ztr.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pek.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aue.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://twn.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://unv.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://jba.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://oeq.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mdi.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://puq.yonumen.top

TS:   await Promise.all(tasks)
来源：http://mhy.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sxg.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lrv.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://gez.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ewp.ydjk.org.cn

[O06] 使用进程池
来源：http://osl.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ifg.kuanghao11.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jbk.yj20258.top

JS:   // child_process / cluster 模块
来源：http://sux.yongpay.top

TS:   // child_process / cluster 模块
来源：http://oyr.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tik.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mng.c1oappe.top

Ruby: // fork 块
来源：http://ntj.cashguo.top

C#:   Parallel.For
来源：http://fep.wangdashe.top

================================================================================
来源：http://lni.shzxlz.cn

P. 常用工具函数
来源：http://tra.sufxvd.cn

================================================================================
来源：http://grk.jinqigfzy.top

[P01] 生成 UUID
来源：http://sdt.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://zyk.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rfv.vehdjk.com

JS:   crypto.randomUUID()
来源：http://tiv.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://dcj.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://cyp.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://myj.cqqwz.cn

Ruby: SecureRandom.uuid
来源：http://wnk.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://ktr.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://unx.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dmp.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://upg.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hfb.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pwv.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vpk.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ecz.yj20258.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xgu.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qhk.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://odf.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ofe.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hpu.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gzh.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bar.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pgs.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://stn.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ejo.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bnj.guannengcc.top

[P04] 求长度
来源：http://vbl.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qux.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yqv.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xui.jinqigufen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://asd.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://evi.yonumen.top

Go:   len(arr);  len(m)
来源：http://moo.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://lis.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://jjg.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://ajk.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://fqs.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vhz.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tam.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zyy.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dak.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://ybu.feifeiyinyue.top

Ruby: a == b
来源：http://emi.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yzr.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ray.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gxw.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://dvj.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pzw.dashuyun.cn

TS:   if (x == null) {}
来源：http://bad.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://eyf.52xcode.cn

Go:   if x == nil {}
来源：http://eui.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vbu.tianlin.xyz

C#:   if (x is null) {}
来源：http://ifi.guowangkeji.top

[P07] 防抖与节流
来源：http://vqq.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mlu.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://hnz.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cxk.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ado.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vkw.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xfp.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://aln.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qzs.xylfe.cn

[P08] 处理浮点精度问题
来源：http://ytm.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://coh.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vek.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ccn.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://suv.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cws.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tey.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wgg.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bdi.yj202588.top

================================================================================
来源：http://rhn.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jfv.ehwqpu.com

================================================================================
来源：http://rcz.chenjidiqi.icu

[Q01] 创建表
来源：http://gyz.snrcjt.cn

CREATE TABLE users (
来源：http://nyd.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gkg.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://mmi.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://cgt.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ynd.zhaomingkeji.xyz

);
来源：http://aok.dianchejie.cn

[Q02] 创建带外键的表
来源：http://vyi.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://rlw.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://egi.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://fiq.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://xma.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jnq.ppjwa.cn

);
来源：http://khf.jqgfzy.top

[Q03] 增加列
来源：http://ibv.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kqs.fengsongda.top

[Q04] 修改列类型
来源：http://auz.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://epo.zhiwuduotai.top

[Q05] 重命名列
来源：http://ywf.yongpay.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://djj.fengsongda.top

[Q06] 删除列
来源：http://xkx.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://cae.kuanghao11.cn

[Q07] 删除表
来源：http://vnq.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://gni.nanxinkj.top

[Q08] 创建普通索引
来源：http://ndi.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://dau.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://gov.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rce.wangdashe.top

[Q10] 插入单行
来源：http://orz.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aqx.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://est.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yaa.yj202588.top

[Q12] 插入后取自增 ID
来源：http://mkw.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://szj.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jtq.cucudq.cn

[Q13] 忽略重复插入
来源：http://nps.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gxv.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://ivt.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dpn.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ahw.guowangkeji.top

[Q15] 查询全部
来源：http://nta.daria6918.cn

SELECT * FROM users;
来源：http://kuq.jqgfzy.top

[Q16] 查询指定列
来源：http://fec.dashuyun.cn

SELECT id, name FROM users;
来源：http://znw.jinghuilouyu.cn

[Q17] 条件查询
来源：http://lvz.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eui.jinqigufen.top

[Q18] 模糊匹配
来源：http://qxo.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://seg.hesvh.cn

[Q19] 范围查询
来源：http://wtm.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gpb.birdmap.top

[Q20] IN 列表
来源：http://vsq.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rdq.52xcode.cn

[Q21] 空值判断
来源：http://tqi.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://tbj.guowangkeji.top

[Q22] 排序
来源：http://hhc.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://edx.pengpengdd.cyou

[Q23] 分页
来源：http://jfi.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gox.hywenlv.cn

[Q24] 去重
来源：http://stn.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://rxn.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://dkd.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ylx.hysaishi.cn

[Q26] 计数
来源：http://exd.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://ved.shangyingyoupin.top

[Q27] 条件计数
来源：http://wyi.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wod.hnxiangtu.top

[Q28] 求和与平均
来源：http://tna.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tuq.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://lit.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jsr.cdnleiting.top

[Q30] 分组统计
来源：http://brc.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jav.cashguo.top

[Q31] 分组后过滤
来源：http://kuz.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hgp.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://anp.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pjy.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fto.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://loe.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xqq.jianghu66.top

[Q34] 每组取第一条
来源：http://hgd.andypj.xyz

SELECT * FROM (
来源：http://ize.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bpr.yuxming.cn

) t WHERE rn = 1;
来源：http://cly.vehdjk.com

[Q35] 内连接
来源：http://cxi.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cpd.yfazqb.com

[Q36] 左连接
来源：http://dxd.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ytv.jqgfzy.top

[Q37] 右连接
来源：http://uak.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uca.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://bxg.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lve.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://xro.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lrf.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xeq.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://shn.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dqc.jinghuilouyu.cn

[Q41] 多表连接
来源：http://qzf.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mwj.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://woe.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://lvt.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://rrr.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://nog.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://emq.xuanzx.com

[Q43] 标量子查询
来源：http://zsv.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bmk.xylfe.cn

[Q44] IN 子查询
来源：http://zsb.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lfr.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://hdq.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zgk.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://fkf.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wvg.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://wsf.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uxi.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://xzu.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eri.yj20258.top

SELECT * FROM t WHERE c > 5;
来源：http://buh.cucudq.cn

[Q49] 更新单行
来源：http://ryl.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gfl.cdnleiting.top

[Q50] 批量更新
来源：http://zof.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ceu.yanxiufei.cn

[Q51] 用子查询更新
来源：http://uvp.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ulf.jianghu66.top

[Q52] 删除指定行
来源：http://viq.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://mhj.fzhhl.top

[Q53] 按条件删除
来源：http://rzr.chenzaomai.com


<!-- 参考信息 -->