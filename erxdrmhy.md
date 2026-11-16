代发 wailian999

Java: // 手写回溯递归
来源：http://qez.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://xiq.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://gia.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://ddk.c1oappe.top

[N09] 栈与队列
来源：http://ybw.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://frn.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vwc.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://frh.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://umv.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://msb.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ucj.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fyn.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rmh.nwbrower.top

[N10] 链表节点定义
来源：http://dkf.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pvi.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ukg.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fyt.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rtc.yongpay.top

Java: class Node { int v; Node next; }
来源：http://nzm.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://blz.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://alh.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xhr.yj20258.top

[N11] 二叉树中序遍历
来源：http://cls.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nhf.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://qbz.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zxr.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upm.shzxlz.cn

Java: // 手写递归
来源：http://kuj.fzhhl.top

Go:   // 手写递归
来源：http://inu.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dgi.yangfankeji.com

C#:   // 手写递归
来源：http://adf.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aou.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sxk.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lbv.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dnw.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nge.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pzi.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://chd.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dob.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lsm.jinyuanbaomall.cn

================================================================================
来源：http://tfk.zhengqikj.top

O. 并发与异步
来源：http://zsz.yangfankeji.com

================================================================================
来源：http://ssb.wangdashe.top

[O01] 启动一个线程
来源：http://ktw.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://osa.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iyw.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kwa.aizwys.cn

TS:   // 同 JS
来源：http://ivj.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://mpg.zdqjudy.top

Go:   go f()
来源：http://dzt.hammf.cn

Ruby: Thread.new { f }
来源：http://kdn.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://uts.chenzaomai.com

[O02] 使用线程池
来源：http://rcm.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xsz.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mes.c1oappe.top

JS:   // worker_threads 线程池
来源：http://gql.nwbrower.top

TS:   // worker_threads 线程池
来源：http://fob.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://tyf.meibo888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bjl.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aeu.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zrf.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://ocs.gotoacloud.top

Py:   with lock: shared += 1
来源：http://eke.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://czl.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://odn.daria6918.cn

TS:   // 同 JS
来源：http://cts.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://sdh.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mds.jqgufenzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fpj.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://cmm.yj202588.top

[O04] 定义异步函数并等待
来源：http://qkf.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://qqj.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qnf.52xcode.cn

JS:   async function f() { await g(); }
来源：http://nyp.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vmh.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jbe.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iif.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ree.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://vgs.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://kxd.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://cjg.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jbi.fanxiaobao.xyz

JS:   await Promise.all(tasks)
来源：http://mkl.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://qsp.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kjo.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lqe.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://ahk.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oep.yongpay.top

[O06] 使用进程池
来源：http://vnx.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://skf.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qke.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://kig.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://msz.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://diq.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vdv.zycfv.cn

Ruby: // fork 块
来源：http://lsy.pycfn.com

C#:   Parallel.For
来源：http://mld.cashguo.top

================================================================================
来源：http://kqm.zhixingplan.top

P. 常用工具函数
来源：http://pdp.tarul.cn

================================================================================
来源：http://jcp.shzxlz.cn

[P01] 生成 UUID
来源：http://ayi.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://tvr.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pot.yonumen.top

JS:   crypto.randomUUID()
来源：http://smn.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://muh.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://gvo.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://pwc.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://jjh.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://qau.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://gkf.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rsi.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://wca.sweek.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xgo.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iei.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cvx.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cnp.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bwt.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://peo.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://cvc.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rvg.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://adq.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qqu.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kap.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://npk.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uze.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bpy.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dpq.xinyue.icu

[P04] 求长度
来源：http://itw.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://npj.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jdr.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cks.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bha.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://uic.ivvv.top

Go:   len(arr);  len(m)
来源：http://ecg.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://wjr.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jma.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://sho.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zsp.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ytk.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nrg.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xuq.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qvi.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kge.hnxiangtu.top

Ruby: a == b
来源：http://cwd.pycfn.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yed.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pfi.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jtc.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://kut.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://juy.sjlbkw.cn

TS:   if (x == null) {}
来源：http://hzf.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://kgc.nwbrower.top

Go:   if x == nil {}
来源：http://wzv.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tbx.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://etp.kuanghao11.cn

[P07] 防抖与节流
来源：http://nmd.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rai.havefunace.top

PHP:  // 手写时间戳比较
来源：http://vet.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kyq.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgx.bjfxy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gyc.zhengqikj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qcd.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zqc.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fip.hammf.cn

[P08] 处理浮点精度问题
来源：http://san.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wxd.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://onl.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rdf.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yze.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iwu.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zwe.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qbe.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fxh.tanke756.top

================================================================================
来源：http://eom.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rln.guannengcc.top

================================================================================
来源：http://yuo.gotoacloud.top

[Q01] 创建表
来源：http://vru.sufxvd.cn

CREATE TABLE users (
来源：http://zaz.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqh.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://ohy.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://exh.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jtg.zycfv.cn

);
来源：http://pkw.fengsongda.top

[Q02] 创建带外键的表
来源：http://hmn.hywenlv.cn

CREATE TABLE orders (
来源：http://ixt.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gaf.cdnleiting.top

user_id INT NOT NULL,
来源：http://koh.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://cqf.zhaomingkeji.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hpe.jinyuanbaomall.cn

);
来源：http://yur.316326.xyz

[Q03] 增加列
来源：http://fqy.hfpthk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ofv.jqgfzy.top

[Q04] 修改列类型
来源：http://hed.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://suh.ctjpmb.com

[Q05] 重命名列
来源：http://uzd.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lcp.cashguo.top

[Q06] 删除列
来源：http://den.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cxv.hammf.cn

[Q07] 删除表
来源：http://jwl.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://xdn.hnqzz.top

[Q08] 创建普通索引
来源：http://bur.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hcm.andypj.xyz

[Q09] 创建唯一索引
来源：http://nla.jianghu66.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nvb.xylfe.cn

[Q10] 插入单行
来源：http://wjq.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dkw.redwolf501.top

[Q11] 一次插入多行
来源：http://uxz.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nbp.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://rqv.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://jzw.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rua.gzhubu.top

[Q13] 忽略重复插入
来源：http://jkm.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oyz.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://lix.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://czb.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rzo.yj20258.top

[Q15] 查询全部
来源：http://yhv.sufxvd.cn

SELECT * FROM users;
来源：http://mae.cucudq.cn

[Q16] 查询指定列
来源：http://mvr.aibaodan.cn

SELECT id, name FROM users;
来源：http://kvb.ybcxt.top

[Q17] 条件查询
来源：http://gkm.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fuh.yfazqb.com

[Q18] 模糊匹配
来源：http://lfc.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pvo.zycfv.cn

[Q19] 范围查询
来源：http://vhp.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jsw.yj20258.top

[Q20] IN 列表
来源：http://ygf.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://acv.zhixingplan.top

[Q21] 空值判断
来源：http://pua.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://txu.xziqi.cn

[Q22] 排序
来源：http://lzi.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://efx.sweek.top

[Q23] 分页
来源：http://iry.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eok.xuanzx.com

[Q24] 去重
来源：http://trv.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://kdv.aibaodan.cn

[Q25] 只取前 N 条
来源：http://sxi.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rbj.zhiwuduotai.top

[Q26] 计数
来源：http://twu.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://vcq.yfazqb.com

[Q27] 条件计数
来源：http://aoe.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://umh.shangyingyoupin.top

[Q28] 求和与平均
来源：http://qxx.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zgf.hfpthk.cn

[Q29] 最大最小值
来源：http://faz.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pnr.zhiwuduotai.top

[Q30] 分组统计
来源：http://sda.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hya.zhongyouzk.top

[Q31] 分组后过滤
来源：http://iis.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cgd.pycfn.com

[Q32] 分组拼接字符串
来源：http://svv.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hza.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vuk.yvedp.cn

[Q33] 多列分组
来源：http://udf.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kuh.cdnleiting.top

[Q34] 每组取第一条
来源：http://vai.ppjwa.cn

SELECT * FROM (
来源：http://rjk.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://itr.zhongyouzk.top

) t WHERE rn = 1;
来源：http://qnu.cdnleiting.top

[Q35] 内连接
来源：http://vih.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://esn.jqgufenzy.top

[Q36] 左连接
来源：http://lir.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://boa.ydjk.org.cn

[Q37] 右连接
来源：http://hkx.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://utb.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://ytg.yj20258888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zry.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://tsy.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fgh.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gph.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wbn.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lbf.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://zsc.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pff.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://dti.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://hvg.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://ryd.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://oca.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lbp.yonumen.top

[Q43] 标量子查询
来源：http://qff.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jvp.feifeiyinyue.top

[Q44] IN 子查询
来源：http://lyr.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hjy.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://ing.zdqjudy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xsv.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zwq.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xia.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://put.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gyo.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://uul.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rbp.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://nta.zhijiandao.cn

[Q49] 更新单行
来源：http://flx.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://opw.hfpthk.cn

[Q50] 批量更新
来源：http://tsb.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://udw.iojbl.cn

[Q51] 用子查询更新
来源：http://ddc.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fef.ppjwa.cn

[Q52] 删除指定行
来源：http://tjv.sufxvd.cn

DELETE FROM users WHERE id = 10;
来源：http://rkp.c1oappe.top

[Q53] 按条件删除
来源：http://gpa.fengsongda.top


<!-- 参考信息 -->