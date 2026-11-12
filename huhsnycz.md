代发 wailian999

[N09] 栈与队列
来源：http://ucg.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gxn.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ebc.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iiv.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qcj.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ogf.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xyj.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iab.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vqg.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://dgr.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yer.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://xfi.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wpd.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rbz.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://maq.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://lle.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xjv.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rxn.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://cvp.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ufr.aizwys.cn

PHP:  // 手写递归函数
来源：http://rma.sweek.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fsg.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bmp.daxiang520.top

Java: // 手写递归
来源：http://pre.zhijiandao.cn

Go:   // 手写递归
来源：http://xdy.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dej.jiagoushi.top

C#:   // 手写递归
来源：http://pdq.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sbr.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ajd.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wdb.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qns.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tbr.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pna.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://paj.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://htv.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bvv.ywan-chungtsiang.top

================================================================================
来源：http://wij.316326.xyz

O. 并发与异步
来源：http://yzn.uphjek.com

================================================================================
来源：http://wng.sysykeji.top

[O01] 启动一个线程
来源：http://zsp.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wmw.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ijm.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dsk.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://uyq.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://jbh.hcnkem.com

Go:   go f()
来源：http://brh.yvedp.cn

Ruby: Thread.new { f }
来源：http://jzy.yonumen.top

C#:   Task.Run(() => F());
来源：http://nnz.ppjwa.cn

[O02] 使用线程池
来源：http://cnn.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dib.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nmy.ivvv.top

JS:   // worker_threads 线程池
来源：http://xna.havefunace.top

TS:   // worker_threads 线程池
来源：http://pyr.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xjc.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hzx.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mfd.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://psa.ivvv.top

[O03] 加锁保护共享数据
来源：http://knh.fktsv.cn

Py:   with lock: shared += 1
来源：http://zbu.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://ysj.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://huu.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://doh.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://jnp.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://thr.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://cii.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://rus.sysykeji.top

[O04] 定义异步函数并等待
来源：http://etm.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://wwv.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rfg.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://gtq.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nar.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ehy.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dpo.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://esc.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://prx.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://uph.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://qvz.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://joz.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://njd.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://vpa.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kws.wangshuangyany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qun.birdmap.top

Ruby: threads.map(&:join)
来源：http://qim.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hcf.zycfv.cn

[O06] 使用进程池
来源：http://mdw.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tbr.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pnb.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://gxr.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://nju.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qbz.yfazqb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oqp.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://ffb.bjfxy.top

C#:   Parallel.For
来源：http://cjg.52xcode.cn

================================================================================
来源：http://qor.daria6918.cn

P. 常用工具函数
来源：http://aet.snrcjt.cn

================================================================================
来源：http://gfw.0kj1m.cn

[P01] 生成 UUID
来源：http://kjv.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://lwk.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vnp.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://fzy.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://ccz.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://lby.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://vro.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://xyv.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://gor.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://bjx.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yel.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dio.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fms.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jbk.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ebj.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ruz.xuetiantiany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bjd.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lql.smart0.xyz

[P03] 生成短随机字符串
来源：http://kih.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://exi.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kzi.zhongyouzk.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yjm.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://znq.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lmb.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yob.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ppu.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gkm.hywenlv.cn

[P04] 求长度
来源：http://iwh.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hbr.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ucx.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fdn.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jhk.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://chy.yonumen.top

Go:   len(arr);  len(m)
来源：http://kjq.yuanzhike.top

Ruby: x.length;  x.size
来源：http://boe.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qre.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://zvb.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bok.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zpe.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rwg.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yeu.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dzy.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://afz.zhengqikj.top

Ruby: a == b
来源：http://del.52xcode.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dck.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jlx.52xcode.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mhg.guowangkeji.top

PHP:  if (empty($x)) {}
来源：http://gqg.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wzv.yj20258888.top

TS:   if (x == null) {}
来源：http://bjx.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://zhs.zhengqikj.top

Go:   if x == nil {}
来源：http://hjn.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wby.yj20258888.top

C#:   if (x is null) {}
来源：http://dbe.gzhubu.top

[P07] 防抖与节流
来源：http://hob.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ops.uphjek.com

PHP:  // 手写时间戳比较
来源：http://luw.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sle.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qjp.zhijiandao.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://msa.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rpc.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gfv.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ktp.ybcxt.top

[P08] 处理浮点精度问题
来源：http://ive.9152youxi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aiq.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hdu.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dyp.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xxn.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xjr.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pvz.yj20258888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bvb.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qdf.fanxiaobao.xyz

================================================================================
来源：http://qtv.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dlp.yj202588.top

================================================================================
来源：http://qix.fanxiaobao.xyz

[Q01] 创建表
来源：http://mja.fehbvm.com

CREATE TABLE users (
来源：http://jxe.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vik.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://pkx.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://jzb.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://swd.jianghu66.top

);
来源：http://exs.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://ykk.ehwqpu.com

CREATE TABLE orders (
来源：http://fjb.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://axg.shuidangran.top

user_id INT NOT NULL,
来源：http://vco.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://qel.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://psn.jiagoushi.top

);
来源：http://tvx.hesvh.cn

[Q03] 增加列
来源：http://zxp.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jwl.hnqzz.top

[Q04] 修改列类型
来源：http://yix.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yhw.havefunace.top

[Q05] 重命名列
来源：http://amk.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xsf.jianghu66.top

[Q06] 删除列
来源：http://ftk.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://bjx.zhongyouzk.top

[Q07] 删除表
来源：http://qzi.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://fag.shzxlz.cn

[Q08] 创建普通索引
来源：http://aqv.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://swp.sufxvd.cn

[Q09] 创建唯一索引
来源：http://lno.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vaq.yangfankeji.com

[Q10] 插入单行
来源：http://kya.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://foq.fengsongda.top

[Q11] 一次插入多行
来源：http://akc.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ghf.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://jcq.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ufu.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tlf.chenzaomai.com

[Q13] 忽略重复插入
来源：http://kdr.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uhh.yuanzhike.top

[Q14] 存在则更新（upsert）
来源：http://ikj.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nqs.shangyingyoupin.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://juc.jianghu66.top

[Q15] 查询全部
来源：http://ttw.snrcjt.cn

SELECT * FROM users;
来源：http://myy.hnqzz.top

[Q16] 查询指定列
来源：http://ccc.iojbl.cn

SELECT id, name FROM users;
来源：http://ddj.havefunace.top

[Q17] 条件查询
来源：http://lih.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oeh.svipenyu.cn

[Q18] 模糊匹配
来源：http://fyg.chenzaomai.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mib.yj20258.top

[Q19] 范围查询
来源：http://nnf.yj202588.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gif.52xcode.cn

[Q20] IN 列表
来源：http://ncn.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lbd.cqqwz.cn

[Q21] 空值判断
来源：http://net.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mec.yj20258888.top

[Q22] 排序
来源：http://mlo.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xnv.pycfn.com

[Q23] 分页
来源：http://vjj.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bat.zhixingplan.top

[Q24] 去重
来源：http://fnt.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://clc.bbcook.cn

[Q25] 只取前 N 条
来源：http://egw.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ruu.yuxming.cn

[Q26] 计数
来源：http://jea.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://ceu.smart0.xyz

[Q27] 条件计数
来源：http://ake.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cpf.jqgfzy.top

[Q28] 求和与平均
来源：http://xpx.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fjr.yj20258888.top

[Q29] 最大最小值
来源：http://xyp.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://sam.0kj1m.cn

[Q30] 分组统计
来源：http://ior.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fsy.yfazqb.com

[Q31] 分组后过滤
来源：http://uyt.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rce.vehdjk.com

[Q32] 分组拼接字符串
来源：http://gfb.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ffl.smart0.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://grk.fzhhl.top

[Q33] 多列分组
来源：http://eeb.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://erk.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://cvh.mhx1999.top

SELECT * FROM (
来源：http://hwe.chenjidiqi.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hkq.ydjk.org.cn

) t WHERE rn = 1;
来源：http://ihz.fengsongda.top

[Q35] 内连接
来源：http://tdv.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jum.chenjidiqi.icu

[Q36] 左连接
来源：http://uvr.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://noa.cqqwz.cn

[Q37] 右连接
来源：http://dvb.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dta.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tsn.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://edo.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://jzu.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rtz.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nbj.9152youxi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dke.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ogq.yueranfly.top

[Q41] 多表连接
来源：http://fwo.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://wmv.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://zyl.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://lba.cashguo.top

[Q42] 连接条件附加过滤
来源：http://srd.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u
来源：http://npy.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bsw.ydjk.org.cn

[Q43] 标量子查询
来源：http://hjm.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wel.snrcjt.cn

[Q44] IN 子查询
来源：http://hpa.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yde.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://bid.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://srl.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://ivn.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ote.nanxinkj.top

[Q47] 与平均值比较
来源：http://vsf.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://boz.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://kss.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wyj.fengsongda.top

SELECT * FROM t WHERE c > 5;
来源：http://utz.sysykeji.top

[Q49] 更新单行
来源：http://hzc.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vcg.smart0.xyz

[Q50] 批量更新
来源：http://zpm.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://flj.cqqwz.cn

[Q51] 用子查询更新
来源：http://otb.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ref.hnxiangtu.top

[Q52] 删除指定行
来源：http://vwp.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://cvd.xylfe.cn

[Q53] 按条件删除
来源：http://kgr.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vnf.meibo888.top

[Q54] 清空表
来源：http://fdd.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://uex.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://enz.chenjidiqi.icu


<!-- 参考信息 -->