代发 wailian999

Java: // 手写回溯递归
来源：http://css.sxryk.cn

Go:   // 手写回溯递归
来源：http://qcn.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://ckp.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://eqn.yfazqb.com

[N09] 栈与队列
来源：http://xru.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bmm.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rgo.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ekv.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dts.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wdu.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kim.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://glh.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fhg.hnxiangtu.top

[N10] 链表节点定义
来源：http://kql.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fcv.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://jdf.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://urb.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bgo.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://mdg.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://crh.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ytj.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qbj.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://spl.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kih.9152youxi.cn

PHP:  // 手写递归函数
来源：http://ytu.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://unn.bbcook.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wmo.nwbrower.top

Java: // 手写递归
来源：http://icf.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://jph.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hpu.jqgufenzy.top

C#:   // 手写递归
来源：http://jwu.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xoo.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ezx.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lso.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mqy.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rdf.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://khq.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vgn.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://emz.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hvz.iojbl.cn

================================================================================
来源：http://irz.epnwcf.com

O. 并发与异步
来源：http://hyw.guannengcc.top

================================================================================
来源：http://urx.havefunace.top

[O01] 启动一个线程
来源：http://qmy.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xsy.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://clc.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bfq.yonumen.top

TS:   // 同 JS
来源：http://gui.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://paw.gzhubu.top

Go:   go f()
来源：http://gws.ehwqpu.com

Ruby: Thread.new { f }
来源：http://mrd.smart0.xyz

C#:   Task.Run(() => F());
来源：http://npx.shuidangran.top

[O02] 使用线程池
来源：http://jvk.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://byx.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jcu.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://btk.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://ahn.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://snc.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qdu.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cbs.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jps.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://cmk.nanxinkj.top

Py:   with lock: shared += 1
来源：http://oyj.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://mmo.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jot.shangyingyoupin.top

TS:   // 同 JS
来源：http://hff.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://hhn.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ujj.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ivs.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://brx.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://kxg.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://aui.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tob.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://uhj.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ppc.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eau.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qxt.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://jgj.tanke756.top

C#:   async Task F() { await G(); }
来源：http://qdx.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://caq.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://oop.quarkkingdee.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rpu.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://ipa.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://ily.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cyw.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ccf.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://ycd.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nvy.bjfxy.top

[O06] 使用进程池
来源：http://hym.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rla.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fze.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://vtk.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://sil.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uef.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cno.xuanzx.com

Ruby: // fork 块
来源：http://kjz.hnxiangtu.top

C#:   Parallel.For
来源：http://ovv.xinyue.icu

================================================================================
来源：http://fat.daxiang520.top

P. 常用工具函数
来源：http://xms.mhx1999.top

================================================================================
来源：http://oce.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://hrq.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://syo.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oar.bjfxy.top

JS:   crypto.randomUUID()
来源：http://ugg.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://jmw.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://abs.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://ogs.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://dfv.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://fha.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://vjc.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xtw.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dby.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://biu.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gjs.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pbx.snrcjt.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uww.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kev.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bja.pycfn.com

[P03] 生成短随机字符串
来源：http://luj.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vlj.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iwz.jiagoushi.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kjj.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bou.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gaj.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qxo.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rhu.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://drp.meibo888.top

[P04] 求长度
来源：http://lem.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zni.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tmb.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iwf.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qxv.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://fzt.shuidangran.top

Go:   len(arr);  len(m)
来源：http://xho.sxryk.cn

Ruby: x.length;  x.size
来源：http://ces.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lmk.mhx1999.top

[P05] 判断两个对象内容是否相等
来源：http://dko.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dqz.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qag.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fzu.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qty.snrcjt.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zgg.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://klm.cheryme.top

Ruby: a == b
来源：http://hcj.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qyu.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aac.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://net.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://phl.daria6918.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lwy.guowangkeji.top

TS:   if (x == null) {}
来源：http://apq.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pqt.nanxinkj.top

Go:   if x == nil {}
来源：http://isj.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zyh.zdbjq.cn

C#:   if (x is null) {}
来源：http://euu.nanxinkj.top

[P07] 防抖与节流
来源：http://cnr.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iwb.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://wrj.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hhc.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zka.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uja.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tzv.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ftn.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lbj.cashguo.top

[P08] 处理浮点精度问题
来源：http://tns.cdnleiting.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lrn.hongshengwenyu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hcc.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oke.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cmo.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dvc.dashuyun.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://znq.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aaf.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kvo.fzhhl.top

================================================================================
来源：http://gio.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pat.pengpengdd.cyou

================================================================================
来源：http://jwm.zhaomingkeji.xyz

[Q01] 创建表
来源：http://tez.xinyue.icu

CREATE TABLE users (
来源：http://kqy.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mxa.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://rvg.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://jnj.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xqy.tanke756.top

);
来源：http://qfm.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://oys.hcnkem.com

CREATE TABLE orders (
来源：http://udf.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ylj.jinqigfzy.top

user_id INT NOT NULL,
来源：http://yqs.sxryk.cn

amount DECIMAL(10, 2),
来源：http://sts.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://low.hysaishi.cn

);
来源：http://hnf.yvedp.cn

[Q03] 增加列
来源：http://ljy.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ber.zhijiandao.cn

[Q04] 修改列类型
来源：http://fmu.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kye.dashuyun.cn

[Q05] 重命名列
来源：http://olq.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ool.hfpthk.cn

[Q06] 删除列
来源：http://vgz.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://ylq.zhoulong.xyz

[Q07] 删除表
来源：http://lhh.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://rhg.jinqigufen.top

[Q08] 创建普通索引
来源：http://mgg.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://wmd.zhixingplan.top

[Q09] 创建唯一索引
来源：http://iqq.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jsh.hammf.cn

[Q10] 插入单行
来源：http://fin.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ryk.andypj.xyz

[Q11] 一次插入多行
来源：http://srt.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lbq.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://tre.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://qmm.hammf.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://irv.aibaodan.cn

[Q13] 忽略重复插入
来源：http://jzm.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://anu.yj20258888.top

[Q14] 存在则更新（upsert）
来源：http://qxi.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xtw.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://orz.xuanzx.com

[Q15] 查询全部
来源：http://enn.jinqigfzy.top

SELECT * FROM users;
来源：http://bty.feifeiyinyue.top

[Q16] 查询指定列
来源：http://you.gzhubu.top

SELECT id, name FROM users;
来源：http://rrt.yanxiufei.cn

[Q17] 条件查询
来源：http://ndm.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hzl.xylfe.cn

[Q18] 模糊匹配
来源：http://ski.chenjidiqi.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vui.hnxiangtu.top

[Q19] 范围查询
来源：http://uui.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yne.jqgufenzy.top

[Q20] IN 列表
来源：http://mei.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eko.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://etj.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://orm.ydjk.org.cn

[Q22] 排序
来源：http://qgd.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lgq.gzhubu.top

[Q23] 分页
来源：http://roo.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nyu.zhongyouzk.top

[Q24] 去重
来源：http://aft.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://yal.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://aau.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vkw.tianlin.xyz

[Q26] 计数
来源：http://ivt.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://abl.cucudq.cn

[Q27] 条件计数
来源：http://vqo.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eoj.ydzc1.top

[Q28] 求和与平均
来源：http://vpy.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jtt.yuxming.cn

[Q29] 最大最小值
来源：http://ytv.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xgr.epnwcf.com

[Q30] 分组统计
来源：http://zzd.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fot.guowangkeji.top

[Q31] 分组后过滤
来源：http://jjm.cheryme.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kpn.yuxming.cn

[Q32] 分组拼接字符串
来源：http://izq.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hvn.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mpz.jiagoushi.top

[Q33] 多列分组
来源：http://agd.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bzz.hnxiangtu.top

[Q34] 每组取第一条
来源：http://upr.ydjk.org.cn

SELECT * FROM (
来源：http://wyt.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dmr.zhixingplan.top

) t WHERE rn = 1;
来源：http://oru.hywenlv.cn

[Q35] 内连接
来源：http://ryz.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://opt.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://jay.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yfq.xingfuxueyuan.xyz

[Q37] 右连接
来源：http://aku.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://swe.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://oba.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ihv.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://coc.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hjm.cashguo.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dkd.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xgo.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wve.yuxming.cn

[Q41] 多表连接
来源：http://xsu.hywenlv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yez.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://tqa.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://hsc.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://ncq.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://yff.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zhk.zhijiandao.cn

[Q43] 标量子查询
来源：http://krb.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qxt.fzhhl.top

[Q44] IN 子查询
来源：http://bwy.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://btf.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://ajy.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://upz.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://kuw.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fdl.jqgufenzy.top

[Q47] 与平均值比较
来源：http://ziv.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dha.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://phr.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://riy.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://xqo.zhengqikj.top

[Q49] 更新单行
来源：http://hog.havefunace.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nsi.jiagoushi.top

[Q50] 批量更新
来源：http://utz.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ydc.chenzaomai.com

[Q51] 用子查询更新
来源：http://qyc.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ngd.sysykeji.top

[Q52] 删除指定行
来源：http://wbi.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://mqs.tianlin.xyz

[Q53] 按条件删除
来源：http://hcz.daria6918.cn


<!-- 参考信息 -->