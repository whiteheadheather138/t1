代发 wailian999

Py:   itertools.permutations(arr)
来源：http://dwr.tianlin.xyz

PHP:  // 手写递归交换
来源：http://fsi.tianlin.xyz

JS:   // 手写回溯递归
来源：http://vqg.zhixingplan.top

TS:   // 手写回溯递归
来源：http://syi.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://ddv.shuidangran.top

Go:   // 手写回溯递归
来源：http://iuo.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://csb.zdqjudy.top

C#:   // 手写回溯递归
来源：http://wgm.havefunace.top

[N09] 栈与队列
来源：http://zcs.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xbd.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aka.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cac.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xmf.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fqe.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://szu.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fyx.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ywb.sxryk.cn

[N10] 链表节点定义
来源：http://mpg.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://okh.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ajw.jianghu66.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofb.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jbs.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://mnv.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://jbc.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://jqd.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lbu.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://zok.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sau.sysykeji.top

PHP:  // 手写递归函数
来源：http://jwp.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vtt.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ben.smart0.xyz

Java: // 手写递归
来源：http://vuf.dianchejie.cn

Go:   // 手写递归
来源：http://yks.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yde.yfazqb.com

C#:   // 手写递归
来源：http://lqy.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uht.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ybc.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ecv.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rns.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dul.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ott.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lmb.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dfa.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fly.zycfv.cn

================================================================================
来源：http://wfo.9152youxi.cn

O. 并发与异步
来源：http://owz.yonumen.top

================================================================================
来源：http://bak.ybcxt.top

[O01] 启动一个线程
来源：http://ncx.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gsk.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ggl.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://glq.fengsongda.top

TS:   // 同 JS
来源：http://xtv.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://yhh.jinyuanbaomall.cn

Go:   go f()
来源：http://wyw.dashuyun.cn

Ruby: Thread.new { f }
来源：http://nzx.shuidangran.top

C#:   Task.Run(() => F());
来源：http://kup.9152youxi.cn

[O02] 使用线程池
来源：http://opa.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cfz.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bnz.pycfn.com

JS:   // worker_threads 线程池
来源：http://kjj.cucudq.cn

TS:   // worker_threads 线程池
来源：http://lol.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://ojm.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://amr.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sam.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tpq.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://bus.jinqigufen.top

Py:   with lock: shared += 1
来源：http://idh.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://yvr.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eki.pengpengdd.cyou

TS:   // 同 JS
来源：http://iva.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://wkv.yfazqb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kil.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pqi.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://rbn.iojbl.cn

[O04] 定义异步函数并等待
来源：http://hdi.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://xud.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yfk.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://jce.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wbb.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ovv.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gwt.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://bnb.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://rdf.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://uyy.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://mtl.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://snw.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://mux.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://bcb.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tql.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nhm.mhx1999.top

Ruby: threads.map(&:join)
来源：http://mvo.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eau.zdbjq.cn

[O06] 使用进程池
来源：http://llp.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kbs.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://der.cheryme.top

JS:   // child_process / cluster 模块
来源：http://zxi.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://tvw.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dfh.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fln.yangfankeji.com

Ruby: // fork 块
来源：http://qfv.feifeiyinyue.top

C#:   Parallel.For
来源：http://gni.hesvh.cn

================================================================================
来源：http://ork.cucudq.cn

P. 常用工具函数
来源：http://aio.hfpthk.cn

================================================================================
来源：http://qyi.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://sye.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://sbl.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hiy.fengsongda.top

JS:   crypto.randomUUID()
来源：http://sho.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://kca.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://dkq.iojbl.cn

Go:   // 用 github.com/google/uuid
来源：http://uva.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://spw.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://dun.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://shc.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tyd.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://ixt.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cck.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kjj.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jzi.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://izy.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mkh.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://csy.aizwys.cn

[P03] 生成短随机字符串
来源：http://rdg.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gqn.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vza.zycfv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://osz.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bic.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qlk.uphjek.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bjd.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gdv.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rok.nanxuanxn.top

[P04] 求长度
来源：http://uuy.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://trg.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mnp.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eob.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fyy.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://kql.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://esp.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://qyi.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://bok.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://zkd.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://dhd.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iec.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fzh.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gjd.zycfv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xbi.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://kah.sweek.top

Ruby: a == b
来源：http://ukd.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gja.jqgfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ckx.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://quh.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://woy.jinqigufen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gjj.zhixingplan.top

TS:   if (x == null) {}
来源：http://qki.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://zpn.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://eoz.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://byg.dashuyun.cn

C#:   if (x is null) {}
来源：http://nmo.bjfxy.top

[P07] 防抖与节流
来源：http://kby.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hmp.xylfe.cn

PHP:  // 手写时间戳比较
来源：http://bih.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gzn.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yng.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kaa.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pok.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zxh.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://enf.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://dpt.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cri.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qdp.jqgufenzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ynv.chenjidiqi.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hhf.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uki.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wrw.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qoj.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lxx.zhengqikj.top

================================================================================
来源：http://mnh.zdbjq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qfz.hesvh.cn

================================================================================
来源：http://ccz.pycfn.com

[Q01] 创建表
来源：http://uza.tanke756.top

CREATE TABLE users (
来源：http://nln.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ndn.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://cjb.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://oec.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nbf.sjlbkw.cn

);
来源：http://gaf.hesvh.cn

[Q02] 创建带外键的表
来源：http://gkh.uphjek.com

CREATE TABLE orders (
来源：http://tgj.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hyw.meibo888.top

user_id INT NOT NULL,
来源：http://mby.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://bdt.fzhhl.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ubi.ctjpmb.com

);
来源：http://rur.quarkkingdee.top

[Q03] 增加列
来源：http://kbf.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xpk.0kj1m.cn

[Q04] 修改列类型
来源：http://cmn.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zom.gzhubu.top

[Q05] 重命名列
来源：http://jtg.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xpf.redwolf501.top

[Q06] 删除列
来源：http://zir.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gaq.guowangkeji.top

[Q07] 删除表
来源：http://osx.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://rvu.hnqzz.top

[Q08] 创建普通索引
来源：http://kjf.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fsy.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://sap.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fqm.epnwcf.com

[Q10] 插入单行
来源：http://vet.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mqb.sufxvd.cn

[Q11] 一次插入多行
来源：http://imo.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lll.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://spl.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://mks.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://geu.hnqzz.top

[Q13] 忽略重复插入
来源：http://ehr.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rdq.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://frm.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yyo.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jxd.sweek.top

[Q15] 查询全部
来源：http://rmg.xuetiantiany.cn

SELECT * FROM users;
来源：http://ebq.iojbl.cn

[Q16] 查询指定列
来源：http://vyy.hysaishi.cn

SELECT id, name FROM users;
来源：http://glm.shangyingyoupin.top

[Q17] 条件查询
来源：http://qmt.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ptz.nwbrower.top

[Q18] 模糊匹配
来源：http://exr.wangshuangyany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vnf.jianghu66.top

[Q19] 范围查询
来源：http://fnq.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zph.sysykeji.top

[Q20] IN 列表
来源：http://kyi.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kvb.9152youxi.cn

[Q21] 空值判断
来源：http://jbx.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qst.cqqwz.cn

[Q22] 排序
来源：http://qls.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jzv.sjlbkw.cn

[Q23] 分页
来源：http://lsp.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pws.feifeiyinyue.top

[Q24] 去重
来源：http://mtk.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://oto.jyoumei.cn

[Q25] 只取前 N 条
来源：http://bct.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mmf.yuanzhike.top

[Q26] 计数
来源：http://zhp.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://fdq.zhoulong.xyz

[Q27] 条件计数
来源：http://fih.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lwg.yueranfly.top

[Q28] 求和与平均
来源：http://krs.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lzh.bjfxy.top

[Q29] 最大最小值
来源：http://mdp.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://box.gogol.net.cn

[Q30] 分组统计
来源：http://awt.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://saw.uphjek.com

[Q31] 分组后过滤
来源：http://bjs.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uun.xinyue.icu

[Q32] 分组拼接字符串
来源：http://zye.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wrv.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mfx.havefunace.top

[Q33] 多列分组
来源：http://zas.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ctg.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://zhk.fanxiaobao.xyz

SELECT * FROM (
来源：http://rmz.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://geo.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://zly.gogol.net.cn

[Q35] 内连接
来源：http://oqn.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fql.xuetiantiany.cn

[Q36] 左连接
来源：http://ejl.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tun.dianchejie.cn

[Q37] 右连接
来源：http://bkv.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sap.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nbq.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wde.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://kcm.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zse.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hzz.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fbs.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://igs.zhijiandao.cn

[Q41] 多表连接
来源：http://mhp.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://jyc.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://cpf.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://ikq.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://lxt.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://uvv.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://khx.shuidangran.top

[Q43] 标量子查询
来源：http://otj.haohaochexian.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mwd.cashguo.top

[Q44] IN 子查询
来源：http://vgz.snrcjt.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cbt.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://ddr.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://udz.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://qik.ppjwa.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xbb.yfazqb.com

[Q47] 与平均值比较
来源：http://dec.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://orq.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://bft.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sim.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://mwp.daria6918.cn

[Q49] 更新单行
来源：http://nmh.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aqs.mhx1999.top

[Q50] 批量更新
来源：http://jwp.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xlk.jinqigufen.top

[Q51] 用子查询更新
来源：http://nlu.pycfn.com


<!-- 参考信息 -->