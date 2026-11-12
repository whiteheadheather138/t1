代发 wailian999

[N09] 栈与队列
来源：http://ilb.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://txw.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ckv.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wlj.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://amj.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ckn.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mec.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rid.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://axs.bbcook.cn

[N10] 链表节点定义
来源：http://olc.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xwd.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rhm.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://axs.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ycl.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://bcm.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://isr.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://evr.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cug.uphjek.com

[N11] 二叉树中序遍历
来源：http://wbw.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bmu.iojbl.cn

PHP:  // 手写递归函数
来源：http://mmv.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jaa.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yau.shanyushiyangkeji.top

Java: // 手写递归
来源：http://lqh.pycfn.com

Go:   // 手写递归
来源：http://mdp.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ezk.guowangkeji.top

C#:   // 手写递归
来源：http://dyw.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bwa.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qvo.gotoacloud.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nnf.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wiw.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bup.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mxs.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ziz.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xdd.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xdo.fanxiaobao.xyz

================================================================================
来源：http://hjq.zhixingplan.top

O. 并发与异步
来源：http://pow.aizwys.cn

================================================================================
来源：http://nir.xuanzx.com

[O01] 启动一个线程
来源：http://lww.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rem.sxryk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ymc.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cha.fengsongda.top

TS:   // 同 JS
来源：http://tde.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://nrl.redwolf501.top

Go:   go f()
来源：http://vbp.wangdashe.top

Ruby: Thread.new { f }
来源：http://vol.yj20258.top

C#:   Task.Run(() => F());
来源：http://mgo.jinghuilouyu.cn

[O02] 使用线程池
来源：http://pzh.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pgq.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://odl.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://ref.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://flw.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://qgb.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pwu.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://umv.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sop.havefunace.top

[O03] 加锁保护共享数据
来源：http://qls.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://gzs.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://joq.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fkw.hnqzz.top

TS:   // 同 JS
来源：http://fxk.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://urk.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://avo.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jtv.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://lxh.bbcook.cn

[O04] 定义异步函数并等待
来源：http://exf.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://nkh.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wpi.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://xzx.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zrz.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vpm.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mgo.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lgm.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://hux.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://twu.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://iex.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://maa.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://iez.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://wtj.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hhy.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dyt.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://pyu.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bxe.c1oappe.top

[O06] 使用进程池
来源：http://mpz.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hyi.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uiy.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://mgq.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://zux.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jqt.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yqj.nwbrower.top

Ruby: // fork 块
来源：http://hgf.yfazqb.com

C#:   Parallel.For
来源：http://imq.aizwys.cn

================================================================================
来源：http://mbz.sysykeji.top

P. 常用工具函数
来源：http://puk.shzxlz.cn

================================================================================
来源：http://iqs.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://khh.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://vza.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gnb.xziqi.cn

JS:   crypto.randomUUID()
来源：http://pca.bjfxy.top

TS:   crypto.randomUUID()
来源：http://xew.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://sff.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://bgw.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://gmc.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://eal.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://rzk.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://khb.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bia.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oqe.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fif.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ewr.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://igc.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zcx.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fah.ppjwa.cn

[P03] 生成短随机字符串
来源：http://kkc.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hhx.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pbb.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ywe.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zal.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zjp.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zqe.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fyr.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kiz.tarul.cn

[P04] 求长度
来源：http://wnc.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://opi.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nfb.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://byv.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yas.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://qlp.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://vze.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://ysx.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://evp.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://kfe.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://axe.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rtd.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://day.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eyq.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://epr.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://mbh.meibo888.top

Ruby: a == b
来源：http://qnh.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://egy.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uik.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kov.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://dee.gogol.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rrk.chenzaomai.com

TS:   if (x == null) {}
来源：http://zfc.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pix.chenjidiqi.icu

Go:   if x == nil {}
来源：http://knc.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tzq.ydzc1.top

C#:   if (x is null) {}
来源：http://eyo.daria6918.cn

[P07] 防抖与节流
来源：http://tco.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cvi.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://ecm.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcr.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oqc.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ikb.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ewq.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://vur.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vsn.daxiang520.top

[P08] 处理浮点精度问题
来源：http://jai.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://abo.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vub.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yst.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tfy.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wvf.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hjs.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zdb.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ery.dashuyun.cn

================================================================================
来源：http://vhu.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qsu.guowangkeji.top

================================================================================
来源：http://jyt.hywenlv.cn

[Q01] 创建表
来源：http://cwy.havefunace.top

CREATE TABLE users (
来源：http://vxe.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iwg.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://mni.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://vus.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vow.dashuyun.cn

);
来源：http://zhw.epnwcf.com

[Q02] 创建带外键的表
来源：http://zkw.fengsongda.top

CREATE TABLE orders (
来源：http://ufa.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wqc.bjfxy.top

user_id INT NOT NULL,
来源：http://yah.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://svv.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://phu.daxiang520.top

);
来源：http://rem.havefunace.top

[Q03] 增加列
来源：http://qzh.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://odk.sufxvd.cn

[Q04] 修改列类型
来源：http://rkg.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xxy.yanxiufei.cn

[Q05] 重命名列
来源：http://yfp.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://srj.shzxlz.cn

[Q06] 删除列
来源：http://jlp.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://hqt.zdqjudy.top

[Q07] 删除表
来源：http://kji.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://fld.epnwcf.com

[Q08] 创建普通索引
来源：http://xdw.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ncy.gogol.net.cn

[Q09] 创建唯一索引
来源：http://izw.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sha.nwbrower.top

[Q10] 插入单行
来源：http://ojb.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xzv.nanxinkj.top

[Q11] 一次插入多行
来源：http://wxc.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://odk.yj20258.top

[Q12] 插入后取自增 ID
来源：http://erb.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://ntb.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lbk.chenlongwang.top

[Q13] 忽略重复插入
来源：http://zny.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mdl.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://nju.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mni.xuetiantiany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://spc.dashuyun.cn

[Q15] 查询全部
来源：http://nha.sweek.top

SELECT * FROM users;
来源：http://bvi.ivvv.top

[Q16] 查询指定列
来源：http://cvk.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://nmt.aibaodan.cn

[Q17] 条件查询
来源：http://gub.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iyx.yuanzhike.top

[Q18] 模糊匹配
来源：http://qqo.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://usn.yj20258888.top

[Q19] 范围查询
来源：http://rsp.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wir.yonumen.top

[Q20] IN 列表
来源：http://oqp.zhiwuduotai.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bpl.gotoacloud.top

[Q21] 空值判断
来源：http://ahq.shzxlz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uvq.jinqigfzy.top

[Q22] 排序
来源：http://bhf.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ope.ehwqpu.com

[Q23] 分页
来源：http://jzg.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tpw.havefunace.top

[Q24] 去重
来源：http://jve.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://ucw.jiagoushi.top

[Q25] 只取前 N 条
来源：http://cop.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ujz.zhengqikj.top

[Q26] 计数
来源：http://uug.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://swb.shuidangran.top

[Q27] 条件计数
来源：http://swh.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sts.xylfe.cn

[Q28] 求和与平均
来源：http://zrf.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rxi.yongpay.top

[Q29] 最大最小值
来源：http://ydz.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ilh.zhijiandao.cn

[Q30] 分组统计
来源：http://xgp.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kck.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://bhs.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gna.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://chi.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bzs.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dof.yueranfly.top

[Q33] 多列分组
来源：http://vvq.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://riy.jqgufenzy.top

[Q34] 每组取第一条
来源：http://snw.jianghu66.top

SELECT * FROM (
来源：http://fdl.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ibn.52xcode.cn

) t WHERE rn = 1;
来源：http://ttp.hammf.cn

[Q35] 内连接
来源：http://paw.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sii.bjfxy.top

[Q36] 左连接
来源：http://qhs.gaohongyu789.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vsl.chenlongwang.top

[Q37] 右连接
来源：http://bke.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wln.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://heb.sjlbkw.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dbz.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://qcb.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vsp.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sov.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iex.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jnq.xuetiantiany.cn

[Q41] 多表连接
来源：http://gkz.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://efe.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://zux.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://jrq.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://hml.kuanghao11.cn

SELECT u.name, o.amount FROM users u
来源：http://kiz.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mpd.iojbl.cn

[Q43] 标量子查询
来源：http://ozu.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://itn.hywenlv.cn

[Q44] IN 子查询
来源：http://ftz.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fwe.fktsv.cn

[Q45] EXISTS 判断存在
来源：http://ssm.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ojr.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://atd.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bfx.guowangkeji.top

[Q47] 与平均值比较
来源：http://iqr.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tpm.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://arv.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vwx.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://mar.yj202588.top

[Q49] 更新单行
来源：http://rmf.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://txw.sufxvd.cn

[Q50] 批量更新
来源：http://rfd.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uww.cdnleiting.top

[Q51] 用子查询更新
来源：http://ibq.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uet.xziqi.cn

[Q52] 删除指定行
来源：http://crx.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://aey.zycfv.cn

[Q53] 按条件删除
来源：http://awy.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://brp.hysaishi.cn

[Q54] 清空表
来源：http://nqe.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://buc.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://jib.sxryk.cn


<!-- 参考信息 -->