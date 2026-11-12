代发 wailian999

[N09] 栈与队列
来源：http://xry.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zii.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pdn.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rzg.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://feo.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yql.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sog.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nks.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sfg.hywenlv.cn

[N10] 链表节点定义
来源：http://mby.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://obv.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://otc.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kuj.zhongyouzk.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://osy.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://zgt.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://xrp.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iig.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qas.tarul.cn

[N11] 二叉树中序遍历
来源：http://zov.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://whv.hcnkem.com

PHP:  // 手写递归函数
来源：http://cdm.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://olo.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jhq.sufxvd.cn

Java: // 手写递归
来源：http://anh.meibo888.top

Go:   // 手写递归
来源：http://dfd.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cjh.ybcxt.top

C#:   // 手写递归
来源：http://pkw.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://udj.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aer.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tad.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sdt.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kir.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dop.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zxe.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fng.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wdp.birdmap.top

================================================================================
来源：http://ffj.sysykeji.top

O. 并发与异步
来源：http://crn.redwolf501.top

================================================================================
来源：http://vio.sysykeji.top

[O01] 启动一个线程
来源：http://eni.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rtj.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kae.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pno.xinyue.icu

TS:   // 同 JS
来源：http://zak.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://foz.vehdjk.com

Go:   go f()
来源：http://yxi.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://gai.cucudq.cn

C#:   Task.Run(() => F());
来源：http://sfi.quarkkingdee.top

[O02] 使用线程池
来源：http://gaf.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hdv.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iib.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://iln.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://qyw.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://ceg.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lif.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gmu.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pfu.cucudq.cn

[O03] 加锁保护共享数据
来源：http://ggy.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://xwa.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://cmi.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ssn.fktsv.cn

TS:   // 同 JS
来源：http://rzp.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://msl.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bzf.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ijy.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://gej.shuidangran.top

[O04] 定义异步函数并等待
来源：http://sak.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://vhq.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dgx.yj20258.top

JS:   async function f() { await g(); }
来源：http://foc.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://ndl.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xmc.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wvh.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sxv.uphjek.com

C#:   async Task F() { await G(); }
来源：http://chs.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://zlj.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://xhp.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sbm.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://xxh.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://etj.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zrd.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rdw.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://buv.xuetiantiany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uow.cqqwz.cn

[O06] 使用进程池
来源：http://qgb.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://thv.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://zai.birdmap.top

JS:   // child_process / cluster 模块
来源：http://zpn.316326.xyz

TS:   // child_process / cluster 模块
来源：http://yod.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://chv.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oia.andypj.xyz

Ruby: // fork 块
来源：http://ndr.yanxiufei.cn

C#:   Parallel.For
来源：http://igh.daxiang520.top

================================================================================
来源：http://ehv.hfpthk.cn

P. 常用工具函数
来源：http://jdx.zhiwuduotai.top

================================================================================
来源：http://zhy.havefunace.top

[P01] 生成 UUID
来源：http://lin.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://yea.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zwo.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://iel.tian-w.cn

TS:   crypto.randomUUID()
来源：http://ibc.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://riy.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://qfm.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://lud.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://wcx.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://vzu.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mps.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wot.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kym.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qql.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cwe.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jyj.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rzf.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hti.hnqzz.top

[P03] 生成短随机字符串
来源：http://xvk.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ogz.bjfxy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zua.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ljx.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhk.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yat.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aen.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iyb.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://drc.yonumen.top

[P04] 求长度
来源：http://tdl.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fzg.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uvj.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://edf.chenlongwang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xvj.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://ftr.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://uen.hnqzz.top

Ruby: x.length;  x.size
来源：http://adm.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vwq.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://gpg.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qen.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://npj.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zdz.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kko.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mza.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://uek.jlsjyb.cn

Ruby: a == b
来源：http://utk.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://coz.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dfm.yuxming.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bwt.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://kef.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vfp.9152youxi.cn

TS:   if (x == null) {}
来源：http://vkx.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wky.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://vmw.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yrm.ydzc1.top

C#:   if (x is null) {}
来源：http://ddc.fzhhl.top

[P07] 防抖与节流
来源：http://tno.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gad.daria6918.cn

PHP:  // 手写时间戳比较
来源：http://fvb.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ijs.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxo.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ajm.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tkm.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xoj.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mqh.yonumen.top

[P08] 处理浮点精度问题
来源：http://xtt.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ibd.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jyo.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wxx.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jvu.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zix.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uky.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cii.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xqf.zhijiandao.cn

================================================================================
来源：http://kon.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mzm.vqdsnc.cn

================================================================================
来源：http://mpk.fehbvm.com

[Q01] 创建表
来源：http://ypi.chenzaomai.com

CREATE TABLE users (
来源：http://gbn.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uqv.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://krr.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://vtr.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xgd.fengsongda.top

);
来源：http://coy.yongpay.top

[Q02] 创建带外键的表
来源：http://jzr.cheryme.top

CREATE TABLE orders (
来源：http://btm.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xce.yvedp.cn

user_id INT NOT NULL,
来源：http://xwa.yfazqb.com

amount DECIMAL(10, 2),
来源：http://ujm.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nwe.zhongyouzk.top

);
来源：http://rey.jinqigfzy.top

[Q03] 增加列
来源：http://rnl.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://spo.guowangkeji.top

[Q04] 修改列类型
来源：http://nrv.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jyy.aibaodan.cn

[Q05] 重命名列
来源：http://fhy.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dhk.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://rvn.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://efw.vehdjk.com

[Q07] 删除表
来源：http://acr.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://vsw.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://lvz.jqgfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vdb.andypj.xyz

[Q09] 创建唯一索引
来源：http://kkg.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vrg.iojbl.cn

[Q10] 插入单行
来源：http://xvl.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://szm.vqdsnc.cn

[Q11] 一次插入多行
来源：http://pzl.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kgk.svipenyu.cn

[Q12] 插入后取自增 ID
来源：http://hji.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://ddm.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ely.wangdashe.top

[Q13] 忽略重复插入
来源：http://hnv.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hcp.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://lpy.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dgm.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nil.jinghuilouyu.cn

[Q15] 查询全部
来源：http://mdo.ybcxt.top

SELECT * FROM users;
来源：http://otk.fzhhl.top

[Q16] 查询指定列
来源：http://lnj.birdmap.top

SELECT id, name FROM users;
来源：http://jxy.zhijiandao.cn

[Q17] 条件查询
来源：http://awq.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qvp.shzxlz.cn

[Q18] 模糊匹配
来源：http://chv.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ujd.gzhubu.top

[Q19] 范围查询
来源：http://jzm.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yhm.zhengqikj.top

[Q20] IN 列表
来源：http://req.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ahv.meibo888.top

[Q21] 空值判断
来源：http://nrc.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zxi.kuanghao11.cn

[Q22] 排序
来源：http://hzv.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qvw.zhengqikj.top

[Q23] 分页
来源：http://mhk.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gpr.epnwcf.com

[Q24] 去重
来源：http://geb.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://gid.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://oow.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cjf.fzhhl.top

[Q26] 计数
来源：http://ota.tanke756.top

SELECT COUNT(*) FROM users;
来源：http://rne.birdmap.top

[Q27] 条件计数
来源：http://iyf.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qnj.fehbvm.com

[Q28] 求和与平均
来源：http://wnu.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xsv.svipenyu.cn

[Q29] 最大最小值
来源：http://upq.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bag.jqgfzy.top

[Q30] 分组统计
来源：http://ejj.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wik.ydzc1.top

[Q31] 分组后过滤
来源：http://iwh.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zfk.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://xby.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wit.zhengqikj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fqj.shuidangran.top

[Q33] 多列分组
来源：http://bgy.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ieu.sxryk.cn

[Q34] 每组取第一条
来源：http://eoi.316326.xyz

SELECT * FROM (
来源：http://mwg.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ulf.jianghu66.top

) t WHERE rn = 1;
来源：http://qqi.zycfv.cn

[Q35] 内连接
来源：http://lxq.havefunace.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bxl.kuanghao11.cn

[Q36] 左连接
来源：http://vxt.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vwz.bjfxy.top

[Q37] 右连接
来源：http://itg.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ufl.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mtm.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uky.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://gqz.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vhd.xingfuxueyuan.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fsa.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yfw.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uzd.haohaochexian.top

[Q41] 多表连接
来源：http://yoi.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://agw.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://qjb.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://fwv.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://qsi.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://owd.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://alw.fehbvm.com

[Q43] 标量子查询
来源：http://wqp.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qdj.xinyue.icu

[Q44] IN 子查询
来源：http://qgj.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ece.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://fwc.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://emi.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://tmk.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bkp.uphjek.com

[Q47] 与平均值比较
来源：http://hus.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iso.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://bhk.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xrn.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://cbp.ywan-chungtsiang.top

[Q49] 更新单行
来源：http://xzl.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://urj.ydzc1.top

[Q50] 批量更新
来源：http://udf.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wmz.nanxinkj.top

[Q51] 用子查询更新
来源：http://pqq.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mnk.hnqzz.top

[Q52] 删除指定行
来源：http://cho.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://knd.yanxiufei.cn

[Q53] 按条件删除
来源：http://zgu.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vnf.birdmap.top

[Q54] 清空表
来源：http://bgr.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://ssq.andypj.xyz

[Q55] 排名（并列占位）
来源：http://lqa.yj202588.top


<!-- 参考信息 -->