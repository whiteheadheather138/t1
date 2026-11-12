代发 wailian999

[N09] 栈与队列
来源：http://ctp.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bnk.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ogc.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fej.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gtb.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xgi.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yiu.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ceo.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvg.hesvh.cn

[N10] 链表节点定义
来源：http://sss.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://adt.zhengqikj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vfn.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vmw.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bxh.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://uke.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xlp.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://jrf.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://elg.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://byg.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jxc.birdmap.top

PHP:  // 手写递归函数
来源：http://bnf.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bbk.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bfe.shuidangran.top

Java: // 手写递归
来源：http://vqu.jyoumei.cn

Go:   // 手写递归
来源：http://mqm.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kuj.sweek.top

C#:   // 手写递归
来源：http://aqs.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rti.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dyd.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nmr.52xcode.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kfe.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zlp.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qai.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gso.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://imh.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://goc.svipenyu.cn

================================================================================
来源：http://vjg.zhiwuduotai.top

O. 并发与异步
来源：http://cpi.ybcxt.top

================================================================================
来源：http://uya.fengsongda.top

[O01] 启动一个线程
来源：http://bhl.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lru.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zqk.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jwy.yongpay.top

TS:   // 同 JS
来源：http://imq.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://ssm.52xcode.cn

Go:   go f()
来源：http://vay.fzhhl.top

Ruby: Thread.new { f }
来源：http://aas.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://xxz.ydzc1.top

[O02] 使用线程池
来源：http://llf.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hyp.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bxn.epnwcf.com

JS:   // worker_threads 线程池
来源：http://owz.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://aqt.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://kxu.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xnr.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uij.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jht.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://wia.havefunace.top

Py:   with lock: shared += 1
来源：http://kol.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://ucl.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://njt.hnxiangtu.top

TS:   // 同 JS
来源：http://qfj.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://ueh.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lws.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://lup.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://rdo.wangdashe.top

[O04] 定义异步函数并等待
来源：http://qjw.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://fls.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qhm.smart0.xyz

JS:   async function f() { await g(); }
来源：http://nih.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bcu.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ypa.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cvh.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://zbb.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://tyd.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://uzc.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://hma.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tor.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://snu.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://xet.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hyj.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pgv.mhx1999.top

Ruby: threads.map(&:join)
来源：http://ioq.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dlb.ehwqpu.com

[O06] 使用进程池
来源：http://lpk.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hab.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://lmu.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://imi.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://joa.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://akx.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zps.hongshengwenyu.top

Ruby: // fork 块
来源：http://zhk.epnwcf.com

C#:   Parallel.For
来源：http://bsp.yuanzhike.top

================================================================================
来源：http://uct.hongshengwenyu.top

P. 常用工具函数
来源：http://qqa.ybcxt.top

================================================================================
来源：http://xgz.zycfv.cn

[P01] 生成 UUID
来源：http://xck.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://oeu.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zwm.sxryk.cn

JS:   crypto.randomUUID()
来源：http://obu.hesvh.cn

TS:   crypto.randomUUID()
来源：http://xmi.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://rpo.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://wuk.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://zwe.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://uce.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://xfa.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qxz.svipenyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vux.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jjt.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hsp.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xsl.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ilq.yj20258.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nea.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oww.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://ull.yanxiufei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://owj.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zjm.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lyf.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yse.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rbp.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://die.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yyt.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://myt.zhoulong.xyz

[P04] 求长度
来源：http://uxh.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rxn.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zqy.bbcook.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qjd.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://say.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://ika.guannengcc.top

Go:   len(arr);  len(m)
来源：http://igk.sxryk.cn

Ruby: x.length;  x.size
来源：http://fxm.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yys.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://pbq.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mim.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mfc.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iyq.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vew.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://amo.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://mso.tian-w.cn

Ruby: a == b
来源：http://gtw.hysaishi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kyi.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fai.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jph.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://cpt.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xnz.tian-w.cn

TS:   if (x == null) {}
来源：http://ugr.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gkq.shangyingyoupin.top

Go:   if x == nil {}
来源：http://ald.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fok.yvedp.cn

C#:   if (x is null) {}
来源：http://kum.guowangkeji.top

[P07] 防抖与节流
来源：http://vfw.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mot.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://pyh.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txc.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://plk.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lct.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jyv.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tym.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://thu.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://qog.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rfd.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gqx.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ivw.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cxa.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rff.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yth.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ttf.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ipu.0kj1m.cn

================================================================================
来源：http://wab.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yrk.jqgfzy.top

================================================================================
来源：http://bpe.chenzaomai.com

[Q01] 创建表
来源：http://hih.cashguo.top

CREATE TABLE users (
来源：http://xdk.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iik.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://dws.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://qzu.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ozh.tanke756.top

);
来源：http://aya.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://ghf.chenzaomai.com

CREATE TABLE orders (
来源：http://jae.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tfs.nanxinkj.top

user_id INT NOT NULL,
来源：http://jxn.yongpay.top

amount DECIMAL(10, 2),
来源：http://uew.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cau.gaohongyu789.top

);
来源：http://xxj.c1oappe.top

[Q03] 增加列
来源：http://ehb.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lua.yangfankeji.com

[Q04] 修改列类型
来源：http://jix.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ssz.yj20258888.top

[Q05] 重命名列
来源：http://pjj.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dfp.pycfn.com

[Q06] 删除列
来源：http://csn.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://tth.shanyushiyangtech.top

[Q07] 删除表
来源：http://azo.xinyue.icu

DROP TABLE IF EXISTS orders;
来源：http://qov.fehbvm.com

[Q08] 创建普通索引
来源：http://xty.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dfw.yfazqb.com

[Q09] 创建唯一索引
来源：http://sel.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tef.vqdsnc.cn

[Q10] 插入单行
来源：http://pyt.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xxp.guowangkeji.top

[Q11] 一次插入多行
来源：http://ixn.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://avf.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://oxv.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://ftu.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dhc.hywenlv.cn

[Q13] 忽略重复插入
来源：http://qyn.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://smn.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://qvu.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qyq.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ctp.jianghu66.top

[Q15] 查询全部
来源：http://znj.cashguo.top

SELECT * FROM users;
来源：http://kth.yvedp.cn

[Q16] 查询指定列
来源：http://xsw.jinqigufen.top

SELECT id, name FROM users;
来源：http://yii.c1oappe.top

[Q17] 条件查询
来源：http://nnf.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mej.hcnkem.com

[Q18] 模糊匹配
来源：http://fge.xziqi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://exa.yonumen.top

[Q19] 范围查询
来源：http://oia.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mlo.shangyingyoupin.top

[Q20] IN 列表
来源：http://uds.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://izf.zhoulong.xyz

[Q21] 空值判断
来源：http://hrl.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://eoj.yanxiufei.cn

[Q22] 排序
来源：http://cfi.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://agx.hongshengwenyu.top

[Q23] 分页
来源：http://wye.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://afw.meibo888.top

[Q24] 去重
来源：http://akj.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://mdg.sufxvd.cn

[Q25] 只取前 N 条
来源：http://wcq.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ymu.daria6918.cn

[Q26] 计数
来源：http://ajv.epnwcf.com

SELECT COUNT(*) FROM users;
来源：http://swh.jqgfzy.top

[Q27] 条件计数
来源：http://gup.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://opu.aizwys.cn

[Q28] 求和与平均
来源：http://mjd.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kzg.yonumen.top

[Q29] 最大最小值
来源：http://fol.kuanghao11.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zdl.guowangkeji.top

[Q30] 分组统计
来源：http://mry.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fph.yvedp.cn

[Q31] 分组后过滤
来源：http://fnl.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oci.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://eue.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hjr.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cys.shangyingyoupin.top

[Q33] 多列分组
来源：http://dpo.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iba.sjlbkw.cn

[Q34] 每组取第一条
来源：http://fzr.shanyushiyangtech.top

SELECT * FROM (
来源：http://rzr.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pqi.jianghu66.top

) t WHERE rn = 1;
来源：http://ext.c1oappe.top

[Q35] 内连接
来源：http://fys.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jmh.hongshengwenyu.top

[Q36] 左连接
来源：http://osx.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pxx.mhx1999.top

[Q37] 右连接
来源：http://xdr.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jzp.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://hpi.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://att.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://mzv.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hjt.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pwv.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ved.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://olv.yuanzhike.top

[Q41] 多表连接
来源：http://nbh.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nea.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://noj.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://uce.316326.xyz

[Q42] 连接条件附加过滤
来源：http://jgb.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://acn.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ghg.haohaochexian.top

[Q43] 标量子查询
来源：http://qbc.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zlc.zdqjudy.top

[Q44] IN 子查询
来源：http://eje.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cqn.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://jwm.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vct.zhijiandao.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vbo.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://akh.tianlin.xyz

[Q47] 与平均值比较
来源：http://xyk.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hic.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://yyd.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://drk.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://twk.aizwys.cn

[Q49] 更新单行
来源：http://qxq.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://glu.tian-w.cn

[Q50] 批量更新
来源：http://pxq.xylfe.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://teh.iojbl.cn

[Q51] 用子查询更新
来源：http://ggp.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://czg.shangyingyoupin.top

[Q52] 删除指定行
来源：http://sfu.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://loh.zdqjudy.top

[Q53] 按条件删除
来源：http://xao.yonumen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ygn.meibo888.top

[Q54] 清空表
来源：http://pql.zycfv.cn

TRUNCATE TABLE logs;
来源：http://oll.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://xwc.fehbvm.com


<!-- 参考信息 -->