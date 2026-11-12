代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pah.zdbjq.cn

[N10] 链表节点定义
来源：http://ylu.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vnb.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mrj.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vmc.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rgz.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://fnw.ppjwa.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mdo.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://alu.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uev.uphjek.com

[N11] 二叉树中序遍历
来源：http://lhn.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zip.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://eag.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gwb.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uut.cdnleiting.top

Java: // 手写递归
来源：http://vdo.jyoumei.cn

Go:   // 手写递归
来源：http://ogh.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kfr.smart0.xyz

C#:   // 手写递归
来源：http://ftu.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ujf.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://siw.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bbo.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://noe.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gpw.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://euj.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lrm.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oto.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://spn.zhixingplan.top

================================================================================
来源：http://oeq.hywenlv.cn

O. 并发与异步
来源：http://xfy.ivvv.top

================================================================================
来源：http://wlm.vehdjk.com

[O01] 启动一个线程
来源：http://kvr.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zru.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nkl.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ddx.daxiang520.top

TS:   // 同 JS
来源：http://bav.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://iis.zycfv.cn

Go:   go f()
来源：http://jdt.yj202588.top

Ruby: Thread.new { f }
来源：http://sgv.sxryk.cn

C#:   Task.Run(() => F());
来源：http://qsw.shangyingyoupin.top

[O02] 使用线程池
来源：http://cuf.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dhf.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kbh.52xcode.cn

JS:   // worker_threads 线程池
来源：http://jgu.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://qxf.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gwb.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ajd.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qgg.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iun.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://ete.jianghu66.top

Py:   with lock: shared += 1
来源：http://kxv.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://gvi.vqdsnc.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fsh.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://ars.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://pph.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iqd.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yqe.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://vhd.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://kha.gotoacloud.top

Py:   async def f():⏎    await g()
来源：http://tas.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jsz.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://sho.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fgs.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hhy.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tpm.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://byu.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://ffn.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://tdu.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://csr.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://flh.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://jgg.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://pdw.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jjf.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://txv.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://foi.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kwl.mhx1999.top

[O06] 使用进程池
来源：http://adg.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zbt.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://apv.hcnkem.com

JS:   // child_process / cluster 模块
来源：http://ijr.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://nyr.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vbm.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://src.yj20258888.top

Ruby: // fork 块
来源：http://vck.cheryme.top

C#:   Parallel.For
来源：http://rph.svipenyu.cn

================================================================================
来源：http://mpx.chenlongwang.top

P. 常用工具函数
来源：http://lll.vqdsnc.cn

================================================================================
来源：http://glt.hnqzz.top

[P01] 生成 UUID
来源：http://qwi.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://opv.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://svx.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://tig.shanyushiyangkeji.top

TS:   crypto.randomUUID()
来源：http://pbe.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://gmj.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://tis.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://voz.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://adm.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://qjx.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://onn.xinyue.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://pll.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ysl.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://guq.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uyv.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ryl.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kvr.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kze.xinyue.icu

[P03] 生成短随机字符串
来源：http://med.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hga.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gdj.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbt.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://avt.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://icn.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mtw.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dff.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://puk.cheryme.top

[P04] 求长度
来源：http://ewh.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ugq.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sqh.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ewj.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hze.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://dpt.daria6918.cn

Go:   len(arr);  len(m)
来源：http://yuv.shuidangran.top

Ruby: x.length;  x.size
来源：http://bkf.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pqj.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://jsz.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lan.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nfg.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rbh.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://idk.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uws.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://wkb.fengsongda.top

Ruby: a == b
来源：http://mjq.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://odi.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://inc.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aaj.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://qmp.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://idl.52xcode.cn

TS:   if (x == null) {}
来源：http://wxj.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nec.daria6918.cn

Go:   if x == nil {}
来源：http://vvi.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tjt.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://xjp.smart0.xyz

[P07] 防抖与节流
来源：http://iyb.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hft.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://yup.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azq.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixq.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wdt.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gdw.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://exh.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aal.uphjek.com

[P08] 处理浮点精度问题
来源：http://efo.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zhe.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yfi.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pji.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://puc.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vqz.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gjt.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lkm.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uoi.uphjek.com

================================================================================
来源：http://xzm.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yrl.jlsjyb.cn

================================================================================
来源：http://ugv.jianghu66.top

[Q01] 创建表
来源：http://txi.cucudq.cn

CREATE TABLE users (
来源：http://wpy.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://etk.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://tgi.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://enu.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vcl.zhijiandao.cn

);
来源：http://ely.jyoumei.cn

[Q02] 创建带外键的表
来源：http://pph.hcnkem.com

CREATE TABLE orders (
来源：http://byb.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vhp.gaohongyu789.top

user_id INT NOT NULL,
来源：http://vzs.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://jyp.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ysy.bjfxy.top

);
来源：http://pnv.fanxiaobao.xyz

[Q03] 增加列
来源：http://sut.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hqo.havefunace.top

[Q04] 修改列类型
来源：http://zjt.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jwk.sweek.top

[Q05] 重命名列
来源：http://pri.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zcd.hongshengwenyu.top

[Q06] 删除列
来源：http://rjl.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://iny.c1oappe.top

[Q07] 删除表
来源：http://uvk.zycfv.cn

DROP TABLE IF EXISTS orders;
来源：http://vxl.gotoacloud.top

[Q08] 创建普通索引
来源：http://zju.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://udv.shuidangran.top

[Q09] 创建唯一索引
来源：http://ntp.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ugt.jiagoushi.top

[Q10] 插入单行
来源：http://xby.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qts.hammf.cn

[Q11] 一次插入多行
来源：http://afh.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wjj.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://vea.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bsf.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uxp.yangfankeji.com

[Q13] 忽略重复插入
来源：http://ioa.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://djw.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://lmu.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://usj.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bmm.yvedp.cn

[Q15] 查询全部
来源：http://tep.vqdsnc.cn

SELECT * FROM users;
来源：http://jkc.aibaodan.cn

[Q16] 查询指定列
来源：http://mrl.jianghu66.top

SELECT id, name FROM users;
来源：http://dpn.shzxlz.cn

[Q17] 条件查询
来源：http://urb.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://quv.ivvv.top

[Q18] 模糊匹配
来源：http://tgj.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xll.shanyushiyangtech.top

[Q19] 范围查询
来源：http://nxa.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qiv.iojbl.cn

[Q20] IN 列表
来源：http://nqb.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nre.zhoulong.xyz

[Q21] 空值判断
来源：http://ono.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dfq.jinqigufen.top

[Q22] 排序
来源：http://zgj.cheryme.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gmm.sjlbkw.cn

[Q23] 分页
来源：http://mxw.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wdx.cashguo.top

[Q24] 去重
来源：http://hbn.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://csc.haohaochexian.top

[Q25] 只取前 N 条
来源：http://yxy.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aym.yj20258.top

[Q26] 计数
来源：http://nef.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://lyy.ivvv.top

[Q27] 条件计数
来源：http://cim.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qmw.snrcjt.cn

[Q28] 求和与平均
来源：http://nsn.shangyingyoupin.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ecr.jyoumei.cn

[Q29] 最大最小值
来源：http://uya.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gqk.zdqjudy.top

[Q30] 分组统计
来源：http://zqk.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jfr.yuxming.cn

[Q31] 分组后过滤
来源：http://ucs.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oxu.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://vmt.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://how.smart0.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mrd.jiagoushi.top

[Q33] 多列分组
来源：http://lnk.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aoa.yj20258.top

[Q34] 每组取第一条
来源：http://rvz.jqgufenzy.top

SELECT * FROM (
来源：http://fff.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nwf.jinqigfzy.top

) t WHERE rn = 1;
来源：http://hxu.yj20258888.top

[Q35] 内连接
来源：http://oww.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tux.ydjk.org.cn

[Q36] 左连接
来源：http://ipx.gaohongyu789.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://adt.ywan-chungtsiang.top

[Q37] 右连接
来源：http://uza.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fnt.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rka.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tcv.yj202588.top

[Q39] 自连接（查上下级）
来源：http://acy.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ref.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vpg.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://quy.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lid.daxiang520.top

[Q41] 多表连接
来源：http://zjv.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://rra.yonumen.top

JOIN users u ON u.id = o.user_id
来源：http://plf.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://hak.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://wet.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://zfs.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://deu.aizwys.cn

[Q43] 标量子查询
来源：http://opd.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zda.fzhhl.top

[Q44] IN 子查询
来源：http://etg.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iky.dashuyun.cn

[Q45] EXISTS 判断存在
来源：http://ytn.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gvh.fzhhl.top

[Q46] NOT EXISTS 判断不存在
来源：http://vph.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gde.uphjek.com

[Q47] 与平均值比较
来源：http://dkh.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wxf.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://brd.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zpo.jianghu66.top

SELECT * FROM t WHERE c > 5;
来源：http://zqy.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://cih.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yio.c1oappe.top

[Q50] 批量更新
来源：http://rou.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aas.jqgfzy.top

[Q51] 用子查询更新
来源：http://iah.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://shc.uphjek.com

[Q52] 删除指定行
来源：http://rbq.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://nln.ppjwa.cn

[Q53] 按条件删除
来源：http://eoc.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xbu.zhoulong.xyz

[Q54] 清空表
来源：http://zqb.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://ukh.yongpay.top

[Q55] 排名（并列占位）
来源：http://mct.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rii.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://ldx.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ils.yonumen.top

[Q57] 行号
来源：http://sev.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wvw.mhx1999.top

[Q58] 累计求和
来源：http://ksx.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vlq.dashuyun.cn

[Q59] 分组内累计
来源：http://mdf.ppjwa.cn


<!-- 参考信息 -->