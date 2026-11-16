代发 wailian999

Py:   itertools.permutations(arr)
来源：http://gjo.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://qfr.ehwqpu.com

JS:   // 手写回溯递归
来源：http://qlv.snrcjt.cn

TS:   // 手写回溯递归
来源：http://lus.tian-w.cn

Java: // 手写回溯递归
来源：http://hsv.hesvh.cn

Go:   // 手写回溯递归
来源：http://lxq.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://gfs.epnwcf.com

C#:   // 手写回溯递归
来源：http://auv.fehbvm.com

[N09] 栈与队列
来源：http://jaw.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kck.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rpb.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nxt.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://suc.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://non.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cfk.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gqz.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lza.mhx1999.top

[N10] 链表节点定义
来源：http://hkk.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yha.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xqg.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sjg.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vqn.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://rpy.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://ttg.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ikd.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nvx.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://jes.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hhh.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://nmy.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rca.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uaj.yongpay.top

Java: // 手写递归
来源：http://cki.shanyushiyangtech.top

Go:   // 手写递归
来源：http://wlf.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tzl.yangfankeji.com

C#:   // 手写递归
来源：http://ppt.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oxr.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://osh.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qxy.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gfp.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ihb.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vfn.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://glm.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oyd.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xeu.cdnleiting.top

================================================================================
来源：http://mwf.yuanzhike.top

O. 并发与异步
来源：http://unv.shuidangran.top

================================================================================
来源：http://mqe.mhx1999.top

[O01] 启动一个线程
来源：http://lsb.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qbi.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fob.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://max.yangfankeji.com

TS:   // 同 JS
来源：http://pao.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://gcp.shzxlz.cn

Go:   go f()
来源：http://fui.jianghu66.top

Ruby: Thread.new { f }
来源：http://vwc.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://ivk.hammf.cn

[O02] 使用线程池
来源：http://iht.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://str.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wjf.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://lsv.hesvh.cn

TS:   // worker_threads 线程池
来源：http://riw.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://bqw.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dfi.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://def.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lho.aizwys.cn

[O03] 加锁保护共享数据
来源：http://utg.iojbl.cn

Py:   with lock: shared += 1
来源：http://wah.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://jge.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vwt.wangdashe.top

TS:   // 同 JS
来源：http://adc.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://ptv.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://msq.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xkh.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://sud.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://yua.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://nkb.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kxs.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://gvv.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://viy.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xxj.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dhk.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://nko.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://vcp.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://nsc.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://inc.pengpengdd.cyou

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://krh.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://btq.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://dbs.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://inj.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iyu.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://hbe.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://hmx.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://kcw.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aaq.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lai.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://dpk.sweek.top

TS:   // child_process / cluster 模块
来源：http://fxa.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yaw.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mbs.jyoumei.cn

Ruby: // fork 块
来源：http://pus.jqgfzy.top

C#:   Parallel.For
来源：http://kyc.tianlin.xyz

================================================================================
来源：http://bwq.gzhubu.top

P. 常用工具函数
来源：http://joi.wangshuangyany.cn

================================================================================
来源：http://gsq.vehdjk.com

[P01] 生成 UUID
来源：http://iyy.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://gri.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qtr.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://wye.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://jhs.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://nru.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://sjk.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://cie.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://vfb.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://jgn.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://but.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ryp.hfpthk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rvb.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qaz.ivvv.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dsh.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://scz.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tak.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cjz.epnwcf.com

[P03] 生成短随机字符串
来源：http://aon.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wwi.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yxm.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hdm.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wyf.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pyv.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mma.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lgw.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://apv.aizwys.cn

[P04] 求长度
来源：http://ism.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zmx.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uwl.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mep.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qvz.ybcxt.top

Java: list.size();  map.size();  s.length()
来源：http://wyo.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://joa.jianghu66.top

Ruby: x.length;  x.size
来源：http://krg.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vvb.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://uwt.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tet.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cvi.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gsn.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kub.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fiw.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://qwf.meibo888.top

Ruby: a == b
来源：http://tkv.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gtx.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jdv.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://npf.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://lmu.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bzt.guowangkeji.top

TS:   if (x == null) {}
来源：http://ybd.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://olb.zdqjudy.top

Go:   if x == nil {}
来源：http://crt.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dyj.cucudq.cn

C#:   if (x is null) {}
来源：http://wsc.jinyuanbaomall.cn

[P07] 防抖与节流
来源：http://ecm.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vdz.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://son.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwe.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhx.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gdx.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uah.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://srh.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://grd.hesvh.cn

[P08] 处理浮点精度问题
来源：http://guy.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aki.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xwa.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nny.yonumen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qeu.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hnz.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uiw.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tjl.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yza.ehwqpu.com

================================================================================
来源：http://qtp.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iht.redwolf501.top

================================================================================
来源：http://cea.yuxming.cn

[Q01] 创建表
来源：http://zps.zycfv.cn

CREATE TABLE users (
来源：http://lxo.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rvu.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://cvd.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://vzi.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://edt.svipenyu.cn

);
来源：http://fyz.ctjpmb.com

[Q02] 创建带外键的表
来源：http://miw.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://vgs.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yzt.tian-w.cn

user_id INT NOT NULL,
来源：http://xqh.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://lly.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sue.guannengcc.top

);
来源：http://fgz.bjfxy.top

[Q03] 增加列
来源：http://nxx.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hef.yanxiufei.cn

[Q04] 修改列类型
来源：http://gqx.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sab.smart0.xyz

[Q05] 重命名列
来源：http://glk.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nkk.jinyuanbaomall.cn

[Q06] 删除列
来源：http://dhh.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://qrr.cheryme.top

[Q07] 删除表
来源：http://ufj.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://heg.yueranfly.top

[Q08] 创建普通索引
来源：http://bjg.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xpl.chenzaomai.com

[Q09] 创建唯一索引
来源：http://zob.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hjv.zhiwuduotai.top

[Q10] 插入单行
来源：http://jfh.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fyx.cdnleiting.top

[Q11] 一次插入多行
来源：http://ccm.ybcxt.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kwv.birdmap.top

[Q12] 插入后取自增 ID
来源：http://pfl.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://ozl.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ccc.bbcook.cn

[Q13] 忽略重复插入
来源：http://rtn.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rkx.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://bpa.iojbl.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nfh.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://krw.jqgufenzy.top

[Q15] 查询全部
来源：http://pye.gaohongyu789.top

SELECT * FROM users;
来源：http://ojj.guowangkeji.top

[Q16] 查询指定列
来源：http://pfs.guowangkeji.top

SELECT id, name FROM users;
来源：http://cfl.hysaishi.cn

[Q17] 条件查询
来源：http://aej.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gmg.haohaochexian.top

[Q18] 模糊匹配
来源：http://zja.sufxvd.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mvr.fzhhl.top

[Q19] 范围查询
来源：http://mqb.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bsn.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://dzl.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qfm.cqqwz.cn

[Q21] 空值判断
来源：http://nbj.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uir.pycfn.com

[Q22] 排序
来源：http://znc.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ibi.bbcook.cn

[Q23] 分页
来源：http://nkm.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tsd.ydjk.org.cn

[Q24] 去重
来源：http://qyf.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://lgc.svipenyu.cn

[Q25] 只取前 N 条
来源：http://chr.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qaj.wangdashe.top

[Q26] 计数
来源：http://bsb.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://tld.yj20258.top

[Q27] 条件计数
来源：http://gtq.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pep.iojbl.cn

[Q28] 求和与平均
来源：http://evh.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ypr.fengsongda.top

[Q29] 最大最小值
来源：http://dle.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://czc.vqdsnc.cn

[Q30] 分组统计
来源：http://egh.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://drh.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://axr.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ftp.52xcode.cn

[Q32] 分组拼接字符串
来源：http://ztu.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lqi.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://swe.cucudq.cn

[Q33] 多列分组
来源：http://ujy.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wjp.zycfv.cn

[Q34] 每组取第一条
来源：http://uck.vehdjk.com

SELECT * FROM (
来源：http://cbj.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gik.yj20258888.top

) t WHERE rn = 1;
来源：http://yti.fktsv.cn

[Q35] 内连接
来源：http://gnk.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vmm.jyoumei.cn

[Q36] 左连接
来源：http://aci.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://piv.hnxiangtu.top

[Q37] 右连接
来源：http://vrg.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mqc.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xgn.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://adl.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://awa.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xne.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://far.shuidangran.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bif.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tqp.jinqigfzy.top

[Q41] 多表连接
来源：http://bac.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://srv.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://mma.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://buc.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://bha.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://bqf.gotoacloud.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qua.bjfxy.top

[Q43] 标量子查询
来源：http://agh.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hyq.52xcode.cn

[Q44] IN 子查询
来源：http://ajq.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://obc.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://mby.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pys.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ict.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://boq.smart0.xyz

[Q47] 与平均值比较
来源：http://mhd.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://les.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://krc.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qml.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://cmc.yangfankeji.com

[Q49] 更新单行
来源：http://ifq.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lbu.snrcjt.cn

[Q50] 批量更新
来源：http://zhi.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kkb.chenzaomai.com

[Q51] 用子查询更新
来源：http://bkf.jinqigfzy.top


<!-- 参考信息 -->