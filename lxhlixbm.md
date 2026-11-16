代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://inb.jinqigfzy.top

[N10] 链表节点定义
来源：http://pik.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yfz.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://huz.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qpp.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rpl.yj202588.top

Java: class Node { int v; Node next; }
来源：http://mbk.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://alf.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nom.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://siv.meibo888.top

[N11] 二叉树中序遍历
来源：http://edn.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qtj.zhixingplan.top

PHP:  // 手写递归函数
来源：http://rbj.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jwn.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pbe.zhijiandao.cn

Java: // 手写递归
来源：http://yag.wangshuangyany.cn

Go:   // 手写递归
来源：http://nsh.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sqd.havefunace.top

C#:   // 手写递归
来源：http://fse.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zjs.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bou.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mfz.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ubs.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqy.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vwe.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nht.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ekl.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qkp.yj20258.top

================================================================================
来源：http://gmu.ctjpmb.com

O. 并发与异步
来源：http://hdc.ywan-chungtsiang.top

================================================================================
来源：http://luh.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://vqt.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uwj.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://itn.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ihw.yuanzhike.top

TS:   // 同 JS
来源：http://lcq.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://mfh.quarkkingdee.top

Go:   go f()
来源：http://fhn.bbcook.cn

Ruby: Thread.new { f }
来源：http://wmk.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://pvp.mhx1999.top

[O02] 使用线程池
来源：http://fwe.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lwv.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sef.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://qkz.xylfe.cn

TS:   // worker_threads 线程池
来源：http://sgb.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ced.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://adp.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zko.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rcv.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://cls.sxryk.cn

Py:   with lock: shared += 1
来源：http://hfr.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://bcg.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kgr.quarkkingdee.top

TS:   // 同 JS
来源：http://zgm.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://aje.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kwr.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://hqw.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://fvi.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://uob.hammf.cn

Py:   async def f():⏎    await g()
来源：http://fap.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vwe.ybcxt.top

JS:   async function f() { await g(); }
来源：http://itq.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fcs.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bbb.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mmo.aibaodan.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hse.yj20258.top

C#:   async Task F() { await G(); }
来源：http://pcm.jyoumei.cn

[O05] 并发执行并等待全部完成
来源：http://wcm.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://byp.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://clu.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://xek.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://pib.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mjj.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zjq.xziqi.cn

Ruby: threads.map(&:join)
来源：http://uyy.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eyp.havefunace.top

[O06] 使用进程池
来源：http://wci.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://avw.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dld.meibo888.top

JS:   // child_process / cluster 模块
来源：http://boe.shuidangran.top

TS:   // child_process / cluster 模块
来源：http://gmb.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uhb.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://drd.yj20258888.top

Ruby: // fork 块
来源：http://jik.ydzc1.top

C#:   Parallel.For
来源：http://ljh.hesvh.cn

================================================================================
来源：http://nie.tarul.cn

P. 常用工具函数
来源：http://ewx.9152youxi.cn

================================================================================
来源：http://pvb.tarul.cn

[P01] 生成 UUID
来源：http://fhc.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://qkt.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hle.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://rkq.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://qwm.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://rhf.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://cfn.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://vfx.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://rxu.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://nsa.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lbo.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mfg.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jng.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ucy.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xvj.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gks.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mqt.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bha.yueranfly.top

[P03] 生成短随机字符串
来源：http://byo.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tft.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pya.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rlk.sweek.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vhi.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sts.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rgd.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://npm.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zib.zdqjudy.top

[P04] 求长度
来源：http://zti.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xpv.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://beu.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ric.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pra.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://uya.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://pqo.sxryk.cn

Ruby: x.length;  x.size
来源：http://ecr.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xbr.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://ylm.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://elf.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://llc.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rww.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://neo.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ecs.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://juq.fanxiaobao.xyz

Ruby: a == b
来源：http://kgz.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ifi.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://adw.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bbu.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://mth.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wpm.ehwqpu.com

TS:   if (x == null) {}
来源：http://hzr.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://haf.xuanzx.com

Go:   if x == nil {}
来源：http://eax.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oqe.yuxming.cn

C#:   if (x is null) {}
来源：http://alu.mhx1999.top

[P07] 防抖与节流
来源：http://hxv.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://djg.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://yvc.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nfp.fktsv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mej.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rwy.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xqh.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mgi.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oip.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://trx.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://axp.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://was.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ihl.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://axy.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ohy.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ypt.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://npl.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lee.meibo888.top

================================================================================
来源：http://tao.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://psd.quarkkingdee.top

================================================================================
来源：http://mfw.ppjwa.cn

[Q01] 创建表
来源：http://yrc.kuanghao11.cn

CREATE TABLE users (
来源：http://wxo.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsi.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://ixi.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://jvx.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jli.cheryme.top

);
来源：http://jhh.yj20258.top

[Q02] 创建带外键的表
来源：http://rmj.tian-w.cn

CREATE TABLE orders (
来源：http://xpe.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wtz.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://wvg.hnqzz.top

amount DECIMAL(10, 2),
来源：http://dtt.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vyt.ydjk.org.cn

);
来源：http://hit.ywan-chungtsiang.top

[Q03] 增加列
来源：http://wgl.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tgu.zycfv.cn

[Q04] 修改列类型
来源：http://aqc.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dvh.hysaishi.cn

[Q05] 重命名列
来源：http://ghy.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bzs.haohaochexian.top

[Q06] 删除列
来源：http://stt.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://kgi.guannengcc.top

[Q07] 删除表
来源：http://ciy.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://wci.yuxming.cn

[Q08] 创建普通索引
来源：http://cva.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rkc.fehbvm.com

[Q09] 创建唯一索引
来源：http://ksy.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dfm.haohaochexian.top

[Q10] 插入单行
来源：http://yrf.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ren.c1oappe.top

[Q11] 一次插入多行
来源：http://loj.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xnl.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://wcq.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://ucv.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://okv.fengsongda.top

[Q13] 忽略重复插入
来源：http://fpc.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cni.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://amd.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iul.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cnt.dianchejie.cn

[Q15] 查询全部
来源：http://esa.fengsongda.top

SELECT * FROM users;
来源：http://qkn.gogol.net.cn

[Q16] 查询指定列
来源：http://dhb.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://vqc.hongshengwenyu.top

[Q17] 条件查询
来源：http://kps.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://atm.cdnleiting.top

[Q18] 模糊匹配
来源：http://qwm.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dxv.cucudq.cn

[Q19] 范围查询
来源：http://yye.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bdj.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://qrx.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hfs.aizwys.cn

[Q21] 空值判断
来源：http://bqu.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vzc.shzxlz.cn

[Q22] 排序
来源：http://fra.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tdr.jinqigufen.top

[Q23] 分页
来源：http://ukk.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xdr.fengsongda.top

[Q24] 去重
来源：http://wfq.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://xty.jinqigufen.top

[Q25] 只取前 N 条
来源：http://dxt.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fvb.sufxvd.cn

[Q26] 计数
来源：http://tmi.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://sov.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://zvn.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vug.9152youxi.cn

[Q28] 求和与平均
来源：http://btd.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://own.aizwys.cn

[Q29] 最大最小值
来源：http://xxv.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://tao.yuxming.cn

[Q30] 分组统计
来源：http://qug.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://njg.jiagoushi.top

[Q31] 分组后过滤
来源：http://nbt.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xzg.ybcxt.top

[Q32] 分组拼接字符串
来源：http://pil.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://udd.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mvq.chenzaomai.com

[Q33] 多列分组
来源：http://bca.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ptd.yj20258.top

[Q34] 每组取第一条
来源：http://jah.chenzaomai.com

SELECT * FROM (
来源：http://coc.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ejq.yuanzhike.top

) t WHERE rn = 1;
来源：http://flx.shangyingyoupin.top

[Q35] 内连接
来源：http://vvf.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pny.chenzaomai.com

[Q36] 左连接
来源：http://axs.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uvs.shanyushiyangtech.top

[Q37] 右连接
来源：http://dyi.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tdg.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jwr.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://olj.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://xqe.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dtr.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lei.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bqd.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vpb.sjlbkw.cn

[Q41] 多表连接
来源：http://leu.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://owm.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://gyo.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://eml.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://yol.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://ieh.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lnx.meibo888.top

[Q43] 标量子查询
来源：http://epi.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sbj.iojbl.cn

[Q44] IN 子查询
来源：http://eeq.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wdq.c1oappe.top

[Q45] EXISTS 判断存在
来源：http://asv.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zlc.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://lgm.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fni.hesvh.cn

[Q47] 与平均值比较
来源：http://pgh.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zjg.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://uxa.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oas.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://ckl.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://xsp.aizwys.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kyk.svipenyu.cn

[Q50] 批量更新
来源：http://hyf.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hrs.yuxming.cn

[Q51] 用子查询更新
来源：http://cdz.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kkz.9152youxi.cn

[Q52] 删除指定行
来源：http://fut.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://evl.hongshengwenyu.top

[Q53] 按条件删除
来源：http://fno.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xzf.hnqzz.top

[Q54] 清空表
来源：http://vfy.yueranfly.top

TRUNCATE TABLE logs;
来源：http://jxl.daria6918.cn

[Q55] 排名（并列占位）
来源：http://svn.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://unw.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://pqb.yj20258.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yda.daxiang520.top

[Q57] 行号
来源：http://dvd.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://adk.zhixingplan.top

[Q58] 累计求和
来源：http://uni.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ixh.ctjpmb.com

[Q59] 分组内累计
来源：http://pzs.hnxiangtu.top


<!-- 参考信息 -->