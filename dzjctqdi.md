代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bgu.bbcook.cn

[N10] 链表节点定义
来源：http://fgs.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uso.cashguo.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xxw.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vne.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mgx.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://jkm.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://utm.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hqt.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vwc.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://vfg.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hni.ivvv.top

PHP:  // 手写递归函数
来源：http://apx.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tua.sjlbkw.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://quz.aibaodan.cn

Java: // 手写递归
来源：http://pqc.yueranfly.top

Go:   // 手写递归
来源：http://nuj.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dyj.gotoacloud.top

C#:   // 手写递归
来源：http://eyg.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hpr.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yjj.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uwh.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cud.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://try.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gpu.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jns.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ubk.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://osf.aibaodan.cn

================================================================================
来源：http://bdt.ydzc1.top

O. 并发与异步
来源：http://gcx.c1oappe.top

================================================================================
来源：http://hsb.gzhubu.top

[O01] 启动一个线程
来源：http://vwx.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://glt.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zfq.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vql.zhoulong.xyz

TS:   // 同 JS
来源：http://dhi.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://odt.yuanzhike.top

Go:   go f()
来源：http://ttp.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://tmt.ydzc1.top

C#:   Task.Run(() => F());
来源：http://xqc.jinqigufen.top

[O02] 使用线程池
来源：http://rbw.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qhk.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gpp.yfazqb.com

JS:   // worker_threads 线程池
来源：http://sdt.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://bhz.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://ika.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pyd.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lqj.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lmu.yongpay.top

[O03] 加锁保护共享数据
来源：http://uow.hfpthk.cn

Py:   with lock: shared += 1
来源：http://wkp.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://akt.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iph.ctjpmb.com

TS:   // 同 JS
来源：http://ggi.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://ryj.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cmk.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fhl.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://gne.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://sfp.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://xnb.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://frs.pycfn.com

JS:   async function f() { await g(); }
来源：http://wvh.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vvy.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vmp.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kga.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://cuf.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://nes.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://dlb.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://fgq.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zwb.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://wtd.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://vvl.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nrq.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hhz.yj20258888.top

Ruby: threads.map(&:join)
来源：http://hab.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://nml.yonumen.top

[O06] 使用进程池
来源：http://ynb.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ece.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ocf.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://uve.cashguo.top

TS:   // child_process / cluster 模块
来源：http://vou.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lbn.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xog.c1oappe.top

Ruby: // fork 块
来源：http://bkz.yongpay.top

C#:   Parallel.For
来源：http://sdr.yj202588.top

================================================================================
来源：http://rws.svipenyu.cn

P. 常用工具函数
来源：http://chu.sweek.top

================================================================================
来源：http://cwm.jiagoushi.top

[P01] 生成 UUID
来源：http://obc.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://jnh.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bpk.zhengqikj.top

JS:   crypto.randomUUID()
来源：http://icq.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://ebu.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://bnj.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://gsg.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://pzc.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://laz.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://iwy.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lur.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://haj.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hub.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://goz.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kvh.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://phv.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://abr.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qps.ehwqpu.com

[P03] 生成短随机字符串
来源：http://wzk.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aes.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zqv.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oak.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dof.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ycq.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vzh.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://uud.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rxy.snrcjt.cn

[P04] 求长度
来源：http://inm.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://axp.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oic.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wtf.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sph.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://jlf.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://nom.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://hxl.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sst.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://hpc.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://reu.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rtd.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jpm.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ynq.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kgx.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://dya.ppjwa.cn

Ruby: a == b
来源：http://ekp.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bja.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qzo.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hyn.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://igq.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://glm.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://zup.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ghr.jiagoushi.top

Go:   if x == nil {}
来源：http://cqt.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fup.svipenyu.cn

C#:   if (x is null) {}
来源：http://jld.hcnkem.com

[P07] 防抖与节流
来源：http://yid.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eui.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://qah.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ykt.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhq.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tmz.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eop.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://vzg.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mdb.0kj1m.cn

[P08] 处理浮点精度问题
来源：http://aks.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lpy.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://deh.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rry.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sjb.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mzl.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qip.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lda.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bol.yangfankeji.com

================================================================================
来源：http://lgg.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qvh.nwbrower.top

================================================================================
来源：http://nzs.vehdjk.com

[Q01] 创建表
来源：http://hsn.ivvv.top

CREATE TABLE users (
来源：http://jwt.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zxb.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://cru.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://eat.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pyx.cucudq.cn

);
来源：http://eem.hcnkem.com

[Q02] 创建带外键的表
来源：http://tcm.guowangkeji.top

CREATE TABLE orders (
来源：http://dbj.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qub.hnqzz.top

user_id INT NOT NULL,
来源：http://onk.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://uyl.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gme.zhengqikj.top

);
来源：http://vyd.cheryme.top

[Q03] 增加列
来源：http://szr.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yys.gaohongyu789.top

[Q04] 修改列类型
来源：http://uke.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ebz.epnwcf.com

[Q05] 重命名列
来源：http://jvk.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lgp.zhongyouzk.top

[Q06] 删除列
来源：http://yec.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oyk.gzhubu.top

[Q07] 删除表
来源：http://deh.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://mul.quarkkingdee.top

[Q08] 创建普通索引
来源：http://hkk.haohaochexian.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ncr.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://sjm.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://syb.gaohongyu789.top

[Q10] 插入单行
来源：http://rou.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://coh.tianlin.xyz

[Q11] 一次插入多行
来源：http://seb.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ohg.yongpay.top

[Q12] 插入后取自增 ID
来源：http://elp.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://cdw.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sau.xylfe.cn

[Q13] 忽略重复插入
来源：http://hzp.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uaj.yonumen.top

[Q14] 存在则更新（upsert）
来源：http://pou.wangshuangyany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mxp.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dqv.fehbvm.com

[Q15] 查询全部
来源：http://kfw.316326.xyz

SELECT * FROM users;
来源：http://nxo.daria6918.cn

[Q16] 查询指定列
来源：http://qwx.gotoacloud.top

SELECT id, name FROM users;
来源：http://hbn.smart0.xyz

[Q17] 条件查询
来源：http://bqz.yuanzhike.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yma.jqgufenzy.top

[Q18] 模糊匹配
来源：http://gmf.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rij.shuidangran.top

[Q19] 范围查询
来源：http://urs.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rxb.guannengcc.top

[Q20] IN 列表
来源：http://znk.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://txd.zhijiandao.cn

[Q21] 空值判断
来源：http://ufh.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xyg.sysykeji.top

[Q22] 排序
来源：http://ypo.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bpo.fengsongda.top

[Q23] 分页
来源：http://vuw.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hav.shanyushiyangkeji.top

[Q24] 去重
来源：http://etm.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://wxk.yonumen.top

[Q25] 只取前 N 条
来源：http://emz.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://axx.yuanzhike.top

[Q26] 计数
来源：http://pqk.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://xlo.fktsv.cn

[Q27] 条件计数
来源：http://sbw.ivvv.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hkz.0kj1m.cn

[Q28] 求和与平均
来源：http://bca.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dum.yuxming.cn

[Q29] 最大最小值
来源：http://kmu.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://esh.havefunace.top

[Q30] 分组统计
来源：http://goj.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xli.vqdsnc.cn

[Q31] 分组后过滤
来源：http://xce.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://his.vehdjk.com

[Q32] 分组拼接字符串
来源：http://jez.yonumen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qnd.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mfp.chenjidiqi.icu

[Q33] 多列分组
来源：http://utt.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cgc.yvedp.cn

[Q34] 每组取第一条
来源：http://qpn.dashuyun.cn

SELECT * FROM (
来源：http://qlm.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vpi.sjlbkw.cn

) t WHERE rn = 1;
来源：http://zqw.zhaomingkeji.xyz

[Q35] 内连接
来源：http://fbb.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vdz.hysaishi.cn

[Q36] 左连接
来源：http://zvg.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://otd.ydjk.org.cn

[Q37] 右连接
来源：http://bbm.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://efa.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://fxn.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://chz.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://iff.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://iwb.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wot.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kfr.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wke.bjfxy.top

[Q41] 多表连接
来源：http://bhq.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hqr.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://qlg.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://slm.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://wlu.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://rmp.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hkf.bjfxy.top

[Q43] 标量子查询
来源：http://gkm.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uuh.iojbl.cn

[Q44] IN 子查询
来源：http://mpe.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://diy.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://ame.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ypc.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://mnr.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yty.tianlin.xyz

[Q47] 与平均值比较
来源：http://yzk.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kmj.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://skh.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jgt.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://pkj.uphjek.com

[Q49] 更新单行
来源：http://gtt.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zfy.sweek.top

[Q50] 批量更新
来源：http://sck.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://duv.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://cki.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pal.tanke756.top

[Q52] 删除指定行
来源：http://yzn.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://bwo.andypj.xyz

[Q53] 按条件删除
来源：http://vim.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rqh.hywenlv.cn

[Q54] 清空表
来源：http://cor.iojbl.cn

TRUNCATE TABLE logs;
来源：http://eoy.shuidangran.top

[Q55] 排名（并列占位）
来源：http://fbe.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uvr.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://pas.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xpi.aibaodan.cn

[Q57] 行号
来源：http://npy.fanxiaobao.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nde.zhengqikj.top

[Q58] 累计求和
来源：http://znv.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vsj.zhoulong.xyz

[Q59] 分组内累计
来源：http://stq.xuetiantiany.cn


<!-- 参考信息 -->