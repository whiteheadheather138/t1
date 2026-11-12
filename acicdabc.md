代发 wailian999

Java: // 手写回溯递归
来源：http://eah.sweek.top

Go:   // 手写回溯递归
来源：http://ehj.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://evr.hywenlv.cn

C#:   // 手写回溯递归
来源：http://qon.xuanzx.com

[N09] 栈与队列
来源：http://eio.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ssc.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sqf.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qfm.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lnn.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hys.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ijv.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xdn.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://isr.gogol.net.cn

[N10] 链表节点定义
来源：http://vms.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yrz.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nwv.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wnj.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oqj.316326.xyz

Java: class Node { int v; Node next; }
来源：http://dib.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://phg.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nmy.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ypu.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://qxt.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kzg.jinqigufen.top

PHP:  // 手写递归函数
来源：http://tqp.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lst.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wfu.guannengcc.top

Java: // 手写递归
来源：http://uqq.chenjidiqi.icu

Go:   // 手写递归
来源：http://lyo.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://psy.xuetiantiany.cn

C#:   // 手写递归
来源：http://vau.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://upq.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jcx.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wzu.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hfq.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://weo.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rzp.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zhl.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sbp.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bvx.jqgfzy.top

================================================================================
来源：http://epu.jinqigufen.top

O. 并发与异步
来源：http://clr.pycfn.com

================================================================================
来源：http://fmf.chenlongwang.top

[O01] 启动一个线程
来源：http://pfw.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lcc.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iys.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kxs.cheryme.top

TS:   // 同 JS
来源：http://pvb.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://tkj.xingfuxueyuan.xyz

Go:   go f()
来源：http://ldm.shuidangran.top

Ruby: Thread.new { f }
来源：http://njh.fehbvm.com

C#:   Task.Run(() => F());
来源：http://bqm.uphjek.com

[O02] 使用线程池
来源：http://cit.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ywb.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://abu.jianghu66.top

JS:   // worker_threads 线程池
来源：http://ots.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://ezf.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://olj.svipenyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pms.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wgb.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fix.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://oud.hysaishi.cn

Py:   with lock: shared += 1
来源：http://aii.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://dub.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mlq.gaohongyu789.top

TS:   // 同 JS
来源：http://zhb.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://ytt.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://frg.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://csn.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://nwn.hnqzz.top

[O04] 定义异步函数并等待
来源：http://qvr.tarul.cn

Py:   async def f():⏎    await g()
来源：http://qkv.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qay.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://vnm.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mcm.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oej.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uet.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://abn.havefunace.top

C#:   async Task F() { await G(); }
来源：http://uyy.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://wbr.epnwcf.com

Py:   asyncio.gather(*tasks)
来源：http://fha.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ecw.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://hzp.redwolf501.top

TS:   await Promise.all(tasks)
来源：http://cyj.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yje.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tku.sweek.top

Ruby: threads.map(&:join)
来源：http://yri.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xer.cheryme.top

[O06] 使用进程池
来源：http://eyt.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ogq.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://pcy.iojbl.cn

JS:   // child_process / cluster 模块
来源：http://sid.cheryme.top

TS:   // child_process / cluster 模块
来源：http://yig.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xqp.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mew.ppjwa.cn

Ruby: // fork 块
来源：http://zeq.daxiang520.top

C#:   Parallel.For
来源：http://lbz.wangshuangyany.cn

================================================================================
来源：http://qqv.ehwqpu.com

P. 常用工具函数
来源：http://mta.sweek.top

================================================================================
来源：http://qhy.gogol.net.cn

[P01] 生成 UUID
来源：http://ifk.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://rbo.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xmo.ydzc1.top

JS:   crypto.randomUUID()
来源：http://smm.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://ehq.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://zjm.nanxinkj.top

Go:   // 用 github.com/google/uuid
来源：http://mlr.yonumen.top

Ruby: SecureRandom.uuid
来源：http://bvq.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://taz.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://ure.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ocg.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fxf.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gnv.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zsw.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ayv.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aqr.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://emh.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aiu.dianchejie.cn

[P03] 生成短随机字符串
来源：http://xnu.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oai.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zhi.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uww.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mpw.mhx1999.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lps.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ycm.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bhr.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sgj.gotoacloud.top

[P04] 求长度
来源：http://lcc.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cxh.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hpb.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dkd.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nsd.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://als.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://cog.dashuyun.cn

Ruby: x.length;  x.size
来源：http://yqc.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://tsl.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://aln.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sqc.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rxo.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iqd.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qil.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hmg.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ira.ydzc1.top

Ruby: a == b
来源：http://xvg.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ugk.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pap.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://exh.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://akm.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ent.bbcook.cn

TS:   if (x == null) {}
来源：http://nii.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bmv.ydzc1.top

Go:   if x == nil {}
来源：http://nbk.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://czn.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://ipw.daria6918.cn

[P07] 防抖与节流
来源：http://dnx.zhiwuduotai.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iaf.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://ata.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgi.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://asc.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bmk.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pvc.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://emk.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ahp.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://mgw.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yrb.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uyq.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aqi.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xdn.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ocd.0kj1m.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://icf.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sdt.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zwk.jqgufenzy.top

================================================================================
来源：http://ubn.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://csa.zhoulong.xyz

================================================================================
来源：http://vaq.jinqigfzy.top

[Q01] 创建表
来源：http://tmg.smart0.xyz

CREATE TABLE users (
来源：http://are.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gbg.zhiwuduotai.top

name VARCHAR(50) NOT NULL,
来源：http://ros.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://spb.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wbk.ydzc1.top

);
来源：http://alv.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://cyi.yuxming.cn

CREATE TABLE orders (
来源：http://qjx.xuetiantiany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cdz.jqgfzy.top

user_id INT NOT NULL,
来源：http://fln.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://qhu.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eqo.jianghu66.top

);
来源：http://edf.aibaodan.cn

[Q03] 增加列
来源：http://ooc.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ghm.feifeiyinyue.top

[Q04] 修改列类型
来源：http://ytf.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qua.hcnkem.com

[Q05] 重命名列
来源：http://cos.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://guh.shangyingyoupin.top

[Q06] 删除列
来源：http://ngp.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://pvf.gogol.net.cn

[Q07] 删除表
来源：http://bbh.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://czi.hywenlv.cn

[Q08] 创建普通索引
来源：http://ixd.jlsjyb.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wdz.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://gnn.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://meb.sweek.top

[Q10] 插入单行
来源：http://ekz.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qod.zhengqikj.top

[Q11] 一次插入多行
来源：http://srg.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kfx.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://cnp.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://ksc.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vmd.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://wtf.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tvx.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://hla.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zmq.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tjs.yonumen.top

[Q15] 查询全部
来源：http://ypq.hammf.cn

SELECT * FROM users;
来源：http://jmm.jiagoushi.top

[Q16] 查询指定列
来源：http://ris.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://mmu.nanxinkj.top

[Q17] 条件查询
来源：http://avl.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sqv.ydzc1.top

[Q18] 模糊匹配
来源：http://qvn.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zqc.hnqzz.top

[Q19] 范围查询
来源：http://mpx.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ocp.chenzaomai.com

[Q20] IN 列表
来源：http://hfl.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://myp.tianlin.xyz

[Q21] 空值判断
来源：http://wyk.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ihr.yonumen.top

[Q22] 排序
来源：http://icz.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lbc.bbcook.cn

[Q23] 分页
来源：http://sww.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qqw.zhiwuduotai.top

[Q24] 去重
来源：http://gzb.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://nmn.yj202588.top

[Q25] 只取前 N 条
来源：http://kdo.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yso.chenlongwang.top

[Q26] 计数
来源：http://ubm.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://qto.jyoumei.cn

[Q27] 条件计数
来源：http://ien.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tie.cqqwz.cn

[Q28] 求和与平均
来源：http://jnv.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rdw.xuanzx.com

[Q29] 最大最小值
来源：http://oey.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kcc.yvedp.cn

[Q30] 分组统计
来源：http://zfu.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bon.jianghu66.top

[Q31] 分组后过滤
来源：http://aeq.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bqm.xinyue.icu

[Q32] 分组拼接字符串
来源：http://ndi.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vbd.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ucz.smart0.xyz

[Q33] 多列分组
来源：http://ykc.zycfv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xqe.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://qxh.dianchejie.cn

SELECT * FROM (
来源：http://myl.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ryw.ivvv.top

) t WHERE rn = 1;
来源：http://owt.zhijiandao.cn

[Q35] 内连接
来源：http://bbj.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://soq.yonumen.top

[Q36] 左连接
来源：http://jhd.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vqm.zhijiandao.cn

[Q37] 右连接
来源：http://cdn.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jxf.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://qlq.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dvd.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://car.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nah.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ubf.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tkb.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ush.quarkkingdee.top

[Q41] 多表连接
来源：http://vtg.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://rop.yvedp.cn

JOIN users u ON u.id = o.user_id
来源：http://onm.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://dkv.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://nxf.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://puq.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xsl.52xcode.cn

[Q43] 标量子查询
来源：http://oxm.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://djl.jinqigfzy.top

[Q44] IN 子查询
来源：http://ysr.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eke.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://lyn.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yly.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://gkj.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kyh.jinqigfzy.top

[Q47] 与平均值比较
来源：http://dqq.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fda.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://bji.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://whl.smart0.xyz

SELECT * FROM t WHERE c > 5;
来源：http://xjm.shzxlz.cn

[Q49] 更新单行
来源：http://gns.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://frz.havefunace.top

[Q50] 批量更新
来源：http://ogu.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xum.dianchejie.cn

[Q51] 用子查询更新
来源：http://cxp.zhaomingkeji.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hat.jiagoushi.top

[Q52] 删除指定行
来源：http://ydl.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://dis.wangshuangyany.cn

[Q53] 按条件删除
来源：http://yws.yvedp.cn


<!-- 参考信息 -->