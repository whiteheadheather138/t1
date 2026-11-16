代发 wailian999

Java: // 手写回溯递归
来源：http://owg.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://gvq.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://rvb.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://awj.hesvh.cn

[N09] 栈与队列
来源：http://lic.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xze.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fwz.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fgu.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nnz.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ehn.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jyz.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zem.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zuf.yj20258888.top

[N10] 链表节点定义
来源：http://xhs.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jyl.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://zcu.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hcp.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uet.yj20258.top

Java: class Node { int v; Node next; }
来源：http://qrq.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xvy.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uhc.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://tjc.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://mtw.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wgf.jyoumei.cn

PHP:  // 手写递归函数
来源：http://zox.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oen.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oni.pengpengdd.cyou

Java: // 手写递归
来源：http://cea.fzhhl.top

Go:   // 手写递归
来源：http://vcg.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iwx.316326.xyz

C#:   // 手写递归
来源：http://rvu.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://osn.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xfk.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xqk.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iqr.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lcq.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oge.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tqn.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uuv.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mne.xziqi.cn

================================================================================
来源：http://ajv.sjlbkw.cn

O. 并发与异步
来源：http://vot.zhengqikj.top

================================================================================
来源：http://hjh.zhengqikj.top

[O01] 启动一个线程
来源：http://hhf.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://weq.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://opo.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mgm.aibaodan.cn

TS:   // 同 JS
来源：http://ehi.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://txa.smart0.xyz

Go:   go f()
来源：http://zxz.jqgfzy.top

Ruby: Thread.new { f }
来源：http://pwa.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://pcp.zhongyouzk.top

[O02] 使用线程池
来源：http://gzn.cqqwz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vqj.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://avy.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://lmy.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://oeu.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zqe.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dnw.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ebx.yuxming.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sjd.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://sqt.sufxvd.cn

Py:   with lock: shared += 1
来源：http://qtl.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://vfu.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dta.pengpengdd.cyou

TS:   // 同 JS
来源：http://fjv.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://ins.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hlv.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vib.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://uem.hammf.cn

[O04] 定义异步函数并等待
来源：http://mmj.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://qtq.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://djg.xylfe.cn

JS:   async function f() { await g(); }
来源：http://cvq.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qcz.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eko.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://izj.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://tet.pycfn.com

C#:   async Task F() { await G(); }
来源：http://cfk.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://pkd.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://myf.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gak.havefunace.top

JS:   await Promise.all(tasks)
来源：http://nwf.cashguo.top

TS:   await Promise.all(tasks)
来源：http://osf.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pzr.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tzs.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://teq.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qxd.ehwqpu.com

[O06] 使用进程池
来源：http://wsn.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rgj.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://eem.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://zxp.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://tmq.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qii.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cev.hammf.cn

Ruby: // fork 块
来源：http://kdw.bbcook.cn

C#:   Parallel.For
来源：http://faf.fehbvm.com

================================================================================
来源：http://yva.sysykeji.top

P. 常用工具函数
来源：http://dlf.zhixingplan.top

================================================================================
来源：http://hlj.mhx1999.top

[P01] 生成 UUID
来源：http://ois.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://ewv.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mho.yj20258.top

JS:   crypto.randomUUID()
来源：http://zqt.xinyue.icu

TS:   crypto.randomUUID()
来源：http://dxv.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://fdk.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://vhu.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://zwf.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://dyg.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://vbs.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hrl.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ujq.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lnv.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://auj.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ijm.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cht.yj20258.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dyg.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bar.hnqzz.top

[P03] 生成短随机字符串
来源：http://jaa.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yna.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mja.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qnc.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jsf.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://och.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sdh.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vkp.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jtx.yueranfly.top

[P04] 求长度
来源：http://zsu.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lpq.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://smt.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nzq.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rnl.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://dhe.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://nks.jinqigufen.top

Ruby: x.length;  x.size
来源：http://anf.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uel.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://zmh.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://svh.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vkn.jinyuanbaomall.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ibp.52xcode.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oov.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://paw.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wos.yj20258888.top

Ruby: a == b
来源：http://pnj.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ova.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://igo.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xbb.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://tyg.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bna.0kj1m.cn

TS:   if (x == null) {}
来源：http://weh.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wfp.ctjpmb.com

Go:   if x == nil {}
来源：http://qml.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wvs.jqgfzy.top

C#:   if (x is null) {}
来源：http://imo.jlsjyb.cn

[P07] 防抖与节流
来源：http://iwd.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ysg.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://vpm.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lzk.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hro.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tqw.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ciu.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ghc.ydzc1.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fca.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://ouo.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://arv.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wqg.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hxk.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gts.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xjd.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vfl.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zub.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cud.hfpthk.cn

================================================================================
来源：http://wjk.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://var.jinqigufen.top

================================================================================
来源：http://blt.tanke756.top

[Q01] 创建表
来源：http://kzm.hesvh.cn

CREATE TABLE users (
来源：http://pak.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kpx.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://byt.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://fqv.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kot.yueranfly.top

);
来源：http://toa.yongpay.top

[Q02] 创建带外键的表
来源：http://gtn.havefunace.top

CREATE TABLE orders (
来源：http://pjv.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://whl.c1oappe.top

user_id INT NOT NULL,
来源：http://ukq.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://veh.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xod.xuetiantiany.cn

);
来源：http://fcx.fanxiaobao.xyz

[Q03] 增加列
来源：http://scm.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://awa.sjlbkw.cn

[Q04] 修改列类型
来源：http://idz.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nrh.zhijiandao.cn

[Q05] 重命名列
来源：http://wve.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://htk.tian-w.cn

[Q06] 删除列
来源：http://qyp.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://vht.hongshengwenyu.top

[Q07] 删除表
来源：http://cce.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://jqq.yueranfly.top

[Q08] 创建普通索引
来源：http://aiz.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://quz.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://buo.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://emi.sysykeji.top

[Q10] 插入单行
来源：http://bdb.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sii.jqgufenzy.top

[Q11] 一次插入多行
来源：http://xnh.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://swg.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://tgs.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://umb.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ykr.aizwys.cn

[Q13] 忽略重复插入
来源：http://yng.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vcp.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://pod.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oim.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gqb.epnwcf.com

[Q15] 查询全部
来源：http://dbn.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://xiw.yvedp.cn

[Q16] 查询指定列
来源：http://scl.yvedp.cn

SELECT id, name FROM users;
来源：http://pbr.zhiwuduotai.top

[Q17] 条件查询
来源：http://gzk.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qha.yuxming.cn

[Q18] 模糊匹配
来源：http://gyc.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fsv.9152youxi.cn

[Q19] 范围查询
来源：http://bjy.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gnz.nwbrower.top

[Q20] IN 列表
来源：http://bfe.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kil.hfpthk.cn

[Q21] 空值判断
来源：http://two.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aqs.yongpay.top

[Q22] 排序
来源：http://yun.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gcg.nwbrower.top

[Q23] 分页
来源：http://mst.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rjl.bbcook.cn

[Q24] 去重
来源：http://gky.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://uxp.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://dsj.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wvz.ehwqpu.com

[Q26] 计数
来源：http://kie.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://bth.yj202588.top

[Q27] 条件计数
来源：http://hdo.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lph.fzhhl.top

[Q28] 求和与平均
来源：http://fez.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gwm.kuanghao11.cn

[Q29] 最大最小值
来源：http://gaf.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yqs.hcnkem.com

[Q30] 分组统计
来源：http://jxn.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://osv.52xcode.cn

[Q31] 分组后过滤
来源：http://jop.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oan.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://viv.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bza.xziqi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iqs.yfazqb.com

[Q33] 多列分组
来源：http://ejo.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bee.kuanghao11.cn

[Q34] 每组取第一条
来源：http://yyr.tianlin.xyz

SELECT * FROM (
来源：http://jut.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qhd.fzhhl.top

) t WHERE rn = 1;
来源：http://rrw.cdnleiting.top

[Q35] 内连接
来源：http://iyh.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vzy.nanxuanxn.top

[Q36] 左连接
来源：http://tif.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://utm.ydzc1.top

[Q37] 右连接
来源：http://kjy.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fvd.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://ulz.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yld.birdmap.top

[Q39] 自连接（查上下级）
来源：http://ezq.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tkc.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mff.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ixz.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hvt.havefunace.top

[Q41] 多表连接
来源：http://fzy.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gtd.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://lcf.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://ybv.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://tpt.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://awj.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yoi.jlsjyb.cn

[Q43] 标量子查询
来源：http://nae.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lqp.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://qap.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nbq.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://emq.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rja.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sbl.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lyb.yfazqb.com

[Q47] 与平均值比较
来源：http://mbs.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vyw.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://rex.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fdt.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://zuq.tian-w.cn

[Q49] 更新单行
来源：http://yiq.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uhc.chenjidiqi.icu

[Q50] 批量更新
来源：http://yrn.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qan.hnxiangtu.top

[Q51] 用子查询更新
来源：http://qcf.guannengcc.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lzq.hnxiangtu.top

[Q52] 删除指定行
来源：http://ufu.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://vqk.svipenyu.cn

[Q53] 按条件删除
来源：http://xns.ybcxt.top


<!-- 参考信息 -->