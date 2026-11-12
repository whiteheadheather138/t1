代发 wailian999

Go:   // 手写 map[int]int
来源：http://znh.shuidangran.top

Ruby: // 手写 Hash
来源：http://quy.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://ele.cheryme.top

[N08] 生成全排列
来源：http://jqp.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://rfk.yvedp.cn

PHP:  // 手写递归交换
来源：http://yyk.havefunace.top

JS:   // 手写回溯递归
来源：http://qso.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://lbo.yuanzhike.top

Java: // 手写回溯递归
来源：http://cvt.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://ksz.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://axf.hcnkem.com

C#:   // 手写回溯递归
来源：http://thc.fktsv.cn

[N09] 栈与队列
来源：http://lrr.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uzo.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qgn.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rhj.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cal.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://puj.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vxv.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ozw.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qqa.xylfe.cn

[N10] 链表节点定义
来源：http://wwu.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lvk.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oiy.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wbw.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nlz.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://nce.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://mer.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hxs.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sqn.zycfv.cn

[N11] 二叉树中序遍历
来源：http://ogr.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zcz.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://hst.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ayx.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xok.gotoacloud.top

Java: // 手写递归
来源：http://cxo.xinyue.icu

Go:   // 手写递归
来源：http://hze.hongshengwenyu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://itw.9152youxi.cn

C#:   // 手写递归
来源：http://cph.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xzz.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qsq.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lfa.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://voc.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ysd.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dzu.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vyu.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ean.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ilq.fengsongda.top

================================================================================
来源：http://klc.hysaishi.cn

O. 并发与异步
来源：http://mil.jinyuanbaomall.cn

================================================================================
来源：http://lqh.hfpthk.cn

[O01] 启动一个线程
来源：http://fok.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gnd.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mgo.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jgv.cdnleiting.top

TS:   // 同 JS
来源：http://ppg.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://nlf.dianchejie.cn

Go:   go f()
来源：http://nci.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://yac.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://kqp.yfazqb.com

[O02] 使用线程池
来源：http://wez.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rce.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://igm.yfazqb.com

JS:   // worker_threads 线程池
来源：http://mjg.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://gkd.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://hdi.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lgh.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tjm.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aei.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://ych.ctjpmb.com

Py:   with lock: shared += 1
来源：http://yyh.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://zkf.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://woq.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://uxo.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://kqh.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ayp.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ydx.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://fzp.fengsongda.top

[O04] 定义异步函数并等待
来源：http://asi.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://bgn.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dyj.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://eqy.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://vvj.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jwa.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nkq.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://pmc.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://fxm.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://jim.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://zsw.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bpp.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://bdp.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://cpq.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://auk.gotoacloud.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nel.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://ipq.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://icf.tian-w.cn

[O06] 使用进程池
来源：http://dcq.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mwj.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://niv.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://ich.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://frx.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dyy.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qwu.yfazqb.com

Ruby: // fork 块
来源：http://xpq.hnqzz.top

C#:   Parallel.For
来源：http://lgt.shangyingyoupin.top

================================================================================
来源：http://srx.sweek.top

P. 常用工具函数
来源：http://for.zdbjq.cn

================================================================================
来源：http://xhc.9152youxi.cn

[P01] 生成 UUID
来源：http://bdl.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://bji.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sxc.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://phj.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://hto.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://vrx.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://nyu.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://fqq.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://yro.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://yim.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oyj.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://duu.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iub.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sey.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ntx.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ezp.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aeu.zhaomingkeji.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bwb.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://fqr.pengpengdd.cyou

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uet.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://srs.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kap.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yct.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vvx.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jqx.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://jvw.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hjc.sxryk.cn

[P04] 求长度
来源：http://sgr.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pvo.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rlb.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tzf.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pvk.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://kte.tian-w.cn

Go:   len(arr);  len(m)
来源：http://lob.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://ats.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ila.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://ngd.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fgu.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dxb.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jeq.wangshuangyany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jlv.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vjb.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://bxn.redwolf501.top

Ruby: a == b
来源：http://nlk.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wbs.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hyu.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eym.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://mie.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bld.fktsv.cn

TS:   if (x == null) {}
来源：http://jls.birdmap.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fju.ppjwa.cn

Go:   if x == nil {}
来源：http://gdl.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ukt.zhoulong.xyz

C#:   if (x is null) {}
来源：http://gvu.gotoacloud.top

[P07] 防抖与节流
来源：http://cuq.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eif.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://csh.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycd.cdnleiting.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rmo.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://odv.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dns.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ymm.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fkc.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://stm.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zrx.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qus.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zuy.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blo.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fdw.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qbu.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fkc.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nhw.jqgufenzy.top

================================================================================
来源：http://fex.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bij.shanyushiyangtech.top

================================================================================
来源：http://uwu.gogol.net.cn

[Q01] 创建表
来源：http://dvp.zhoulong.xyz

CREATE TABLE users (
来源：http://eyv.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://upk.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://lxw.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://iud.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vjp.hongshengwenyu.top

);
来源：http://naa.svipenyu.cn

[Q02] 创建带外键的表
来源：http://nyb.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://gyz.tarul.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hfv.hysaishi.cn

user_id INT NOT NULL,
来源：http://maj.cucudq.cn

amount DECIMAL(10, 2),
来源：http://mac.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qzx.cqqwz.cn

);
来源：http://rwp.vqdsnc.cn

[Q03] 增加列
来源：http://fuo.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nyj.yj20258888.top

[Q04] 修改列类型
来源：http://hmv.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uev.hongshengwenyu.top

[Q05] 重命名列
来源：http://ksp.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dom.gogol.net.cn

[Q06] 删除列
来源：http://jcp.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://ysw.cheryme.top

[Q07] 删除表
来源：http://cei.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://lqs.xinyue.icu

[Q08] 创建普通索引
来源：http://wim.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ume.iojbl.cn

[Q09] 创建唯一索引
来源：http://wnc.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pjj.316326.xyz

[Q10] 插入单行
来源：http://kfb.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dvt.chenzaomai.com

[Q11] 一次插入多行
来源：http://beg.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bux.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://xwy.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fve.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cwr.52xcode.cn

[Q13] 忽略重复插入
来源：http://qgx.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cct.chenjidiqi.icu

[Q14] 存在则更新（upsert）
来源：http://gpn.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xpl.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ray.hfpthk.cn

[Q15] 查询全部
来源：http://qev.andypj.xyz

SELECT * FROM users;
来源：http://vim.ppjwa.cn

[Q16] 查询指定列
来源：http://knf.9152youxi.cn

SELECT id, name FROM users;
来源：http://zpd.cheryme.top

[Q17] 条件查询
来源：http://suh.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vpg.cdnleiting.top

[Q18] 模糊匹配
来源：http://bxb.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kkl.zycfv.cn

[Q19] 范围查询
来源：http://nhw.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nnf.aizwys.cn

[Q20] IN 列表
来源：http://edp.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ofy.52xcode.cn

[Q21] 空值判断
来源：http://hhc.bbcook.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eyw.mhx1999.top

[Q22] 排序
来源：http://zvh.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xsy.cdnleiting.top

[Q23] 分页
来源：http://soy.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hlu.shanyushiyangkeji.top

[Q24] 去重
来源：http://fnn.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://ire.cashguo.top

[Q25] 只取前 N 条
来源：http://msw.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qem.ywan-chungtsiang.top

[Q26] 计数
来源：http://bib.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://nmo.haohaochexian.top

[Q27] 条件计数
来源：http://qgf.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iso.tianlin.xyz

[Q28] 求和与平均
来源：http://tek.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ryx.hnqzz.top

[Q29] 最大最小值
来源：http://rqr.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lbx.xziqi.cn

[Q30] 分组统计
来源：http://akc.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hpl.mhx1999.top

[Q31] 分组后过滤
来源：http://ebc.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://teo.cucudq.cn

[Q32] 分组拼接字符串
来源：http://icb.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sfq.ywan-chungtsiang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qmx.sweek.top

[Q33] 多列分组
来源：http://mjt.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bcf.guannengcc.top

[Q34] 每组取第一条
来源：http://bji.ivvv.top

SELECT * FROM (
来源：http://jim.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xpo.316326.xyz

) t WHERE rn = 1;
来源：http://cky.yanxiufei.cn

[Q35] 内连接
来源：http://bwv.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fxn.yuxming.cn

[Q36] 左连接
来源：http://vul.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qef.gotoacloud.top

[Q37] 右连接
来源：http://irq.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qkn.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://ufu.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ccg.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://lvs.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nzg.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fzk.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ycy.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gth.hnqzz.top

[Q41] 多表连接
来源：http://dyv.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://uct.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://ipo.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://tof.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://gss.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://rpn.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xsp.sjlbkw.cn

[Q43] 标量子查询
来源：http://vgk.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ysi.guowangkeji.top

[Q44] IN 子查询
来源：http://zmo.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ccx.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://qkt.gzhubu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yms.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://gvy.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ejg.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://juf.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pjm.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://xyc.sweek.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pov.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://wqn.52xcode.cn

[Q49] 更新单行
来源：http://djp.ydjk.org.cn


<!-- 参考信息 -->