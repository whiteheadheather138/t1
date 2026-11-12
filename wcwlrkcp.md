代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ivc.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hot.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://jri.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://zbd.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xfr.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://zei.fengsongda.top

[N11] 二叉树中序遍历
来源：http://oms.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pxr.jyoumei.cn

PHP:  // 手写递归函数
来源：http://wqs.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fdz.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gdj.zhoulong.xyz

Java: // 手写递归
来源：http://tqo.tian-w.cn

Go:   // 手写递归
来源：http://rgk.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xwn.yanxiufei.cn

C#:   // 手写递归
来源：http://gvx.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rte.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rba.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jgz.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wzk.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qly.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vtr.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gup.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hrl.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jnm.jqgufenzy.top

================================================================================
来源：http://rqd.jinqigfzy.top

O. 并发与异步
来源：http://lga.nwbrower.top

================================================================================
来源：http://cpr.sysykeji.top

[O01] 启动一个线程
来源：http://fpg.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nub.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gkc.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zba.yj20258888.top

TS:   // 同 JS
来源：http://rwg.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://hjp.xinyue.icu

Go:   go f()
来源：http://gur.ybcxt.top

Ruby: Thread.new { f }
来源：http://inf.redwolf501.top

C#:   Task.Run(() => F());
来源：http://nmu.pengpengdd.cyou

[O02] 使用线程池
来源：http://uvg.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://scz.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rkn.yfazqb.com

JS:   // worker_threads 线程池
来源：http://mma.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://akb.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lmo.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kcy.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nuk.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lqz.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://qrr.yongpay.top

Py:   with lock: shared += 1
来源：http://iot.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://cky.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://san.dashuyun.cn

TS:   // 同 JS
来源：http://jqi.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://kpr.xuanzx.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ldi.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://cin.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://qot.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://lev.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://snu.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ocu.andypj.xyz

JS:   async function f() { await g(); }
来源：http://vrh.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://igy.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vzh.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bud.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://sze.ivvv.top

C#:   async Task F() { await G(); }
来源：http://hct.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://puw.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://acq.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tko.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://rtr.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://mxx.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pxh.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fyu.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://mpx.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qpi.redwolf501.top

[O06] 使用进程池
来源：http://eeq.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xib.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gft.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://pdv.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://jww.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mus.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qss.bjfxy.top

Ruby: // fork 块
来源：http://hgw.ehwqpu.com

C#:   Parallel.For
来源：http://djf.yvedp.cn

================================================================================
来源：http://uhd.fktsv.cn

P. 常用工具函数
来源：http://pjz.xziqi.cn

================================================================================
来源：http://ekt.sufxvd.cn

[P01] 生成 UUID
来源：http://wmq.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://nce.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bkm.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://fof.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://mns.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://dfv.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://zca.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://vvx.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://zzn.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://psy.hongshengwenyu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://clz.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yyg.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dvv.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mho.uphjek.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fyu.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rjq.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://psi.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ykt.ivvv.top

[P03] 生成短随机字符串
来源：http://aly.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://htf.sufxvd.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ubm.jiagoushi.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vni.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dhu.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nfx.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ias.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://ydw.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sru.dashuyun.cn

[P04] 求长度
来源：http://ayr.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gyd.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://snm.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgu.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://noy.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://aou.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://got.vehdjk.com

Ruby: x.length;  x.size
来源：http://pwo.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://red.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://vwv.sxryk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yyb.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hqa.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yfz.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sjs.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xoe.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://caq.havefunace.top

Ruby: a == b
来源：http://gnc.shangyingyoupin.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hbi.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wdk.pycfn.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lel.guowangkeji.top

PHP:  if (empty($x)) {}
来源：http://wlw.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aco.hfpthk.cn

TS:   if (x == null) {}
来源：http://hiu.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zzy.jianghu66.top

Go:   if x == nil {}
来源：http://gjd.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://div.iojbl.cn

C#:   if (x is null) {}
来源：http://nsw.cheryme.top

[P07] 防抖与节流
来源：http://akf.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fge.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://nve.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qym.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yed.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zmw.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://glb.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mhy.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ivk.yj202588.top

[P08] 处理浮点精度问题
来源：http://keh.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gmj.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://avl.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kbn.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xhk.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vxf.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gfs.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sud.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uzr.havefunace.top

================================================================================
来源：http://asg.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jtm.hesvh.cn

================================================================================
来源：http://dye.yj20258.top

[Q01] 创建表
来源：http://jnc.bbcook.cn

CREATE TABLE users (
来源：http://xns.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nzs.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://bhs.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://mom.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nhd.ywan-chungtsiang.top

);
来源：http://ijp.dianchejie.cn

[Q02] 创建带外键的表
来源：http://jyj.cqqwz.cn

CREATE TABLE orders (
来源：http://sdz.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tuq.ybcxt.top

user_id INT NOT NULL,
来源：http://epl.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://ule.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bhg.cheryme.top

);
来源：http://oyv.shuidangran.top

[Q03] 增加列
来源：http://fam.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hph.meibo888.top

[Q04] 修改列类型
来源：http://wsn.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://esh.gaohongyu789.top

[Q05] 重命名列
来源：http://rvc.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ipv.fktsv.cn

[Q06] 删除列
来源：http://gsf.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://jee.0kj1m.cn

[Q07] 删除表
来源：http://gez.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://tvc.jiagoushi.top

[Q08] 创建普通索引
来源：http://buk.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dgc.smart0.xyz

[Q09] 创建唯一索引
来源：http://ncf.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mup.xziqi.cn

[Q10] 插入单行
来源：http://ghr.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gpo.daxiang520.top

[Q11] 一次插入多行
来源：http://ccm.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://boo.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://new.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://slz.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qhg.tianlin.xyz

[Q13] 忽略重复插入
来源：http://rqu.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jer.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://iog.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bez.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yox.gotoacloud.top

[Q15] 查询全部
来源：http://qcb.pengpengdd.cyou

SELECT * FROM users;
来源：http://ora.gogol.net.cn

[Q16] 查询指定列
来源：http://zcs.tarul.cn

SELECT id, name FROM users;
来源：http://jbw.wangshuangyany.cn

[Q17] 条件查询
来源：http://mcv.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nve.shzxlz.cn

[Q18] 模糊匹配
来源：http://bbl.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lni.xylfe.cn

[Q19] 范围查询
来源：http://div.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nxk.shzxlz.cn

[Q20] IN 列表
来源：http://aya.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wiq.feifeiyinyue.top

[Q21] 空值判断
来源：http://fyr.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pwa.jyoumei.cn

[Q22] 排序
来源：http://pts.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pzs.yangfankeji.com

[Q23] 分页
来源：http://ger.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ugv.zhijiandao.cn

[Q24] 去重
来源：http://szb.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://vhr.hcnkem.com

[Q25] 只取前 N 条
来源：http://urk.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lmo.hfpthk.cn

[Q26] 计数
来源：http://zhg.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://loc.vqdsnc.cn

[Q27] 条件计数
来源：http://bvr.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fpk.gaohongyu789.top

[Q28] 求和与平均
来源：http://lnq.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gqe.chenlongwang.top

[Q29] 最大最小值
来源：http://qyl.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://yuu.hesvh.cn

[Q30] 分组统计
来源：http://doa.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cbz.uphjek.com

[Q31] 分组后过滤
来源：http://ytc.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jvl.jlsjyb.cn

[Q32] 分组拼接字符串
来源：http://ggx.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zuz.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kma.zhiwuduotai.top

[Q33] 多列分组
来源：http://sem.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hct.sufxvd.cn

[Q34] 每组取第一条
来源：http://msd.yuanzhike.top

SELECT * FROM (
来源：http://gcq.quarkkingdee.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kmq.hesvh.cn

) t WHERE rn = 1;
来源：http://ktw.aibaodan.cn

[Q35] 内连接
来源：http://yfq.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rir.fehbvm.com

[Q36] 左连接
来源：http://foe.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://koa.aizwys.cn

[Q37] 右连接
来源：http://ttq.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sax.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://tub.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sce.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://vlc.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nsf.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qvr.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bma.shuidangran.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://grk.zdbjq.cn

[Q41] 多表连接
来源：http://ftu.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tsi.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://fxb.jlsjyb.cn

JOIN products p ON p.id = o.product_id;
来源：http://jeb.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://vhm.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://nzg.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fry.hcnkem.com

[Q43] 标量子查询
来源：http://cin.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vkg.hongshengwenyu.top

[Q44] IN 子查询
来源：http://sxg.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://beu.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://sqo.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gyp.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://ozt.ctjpmb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ifv.hfpthk.cn

[Q47] 与平均值比较
来源：http://wwe.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uza.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://crb.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ofz.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://upe.ybcxt.top

[Q49] 更新单行
来源：http://zhw.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mvw.jinqigfzy.top

[Q50] 批量更新
来源：http://add.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ggx.tian-w.cn

[Q51] 用子查询更新
来源：http://vyr.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vbu.wangshuangyany.cn

[Q52] 删除指定行
来源：http://uyz.svipenyu.cn

DELETE FROM users WHERE id = 10;
来源：http://bij.fengsongda.top

[Q53] 按条件删除
来源：http://xnh.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hbf.daxiang520.top

[Q54] 清空表
来源：http://wby.hammf.cn

TRUNCATE TABLE logs;
来源：http://fmu.fktsv.cn

[Q55] 排名（并列占位）
来源：http://zvh.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zaz.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://gqu.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://par.vqdsnc.cn

[Q57] 行号
来源：http://jqw.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sqc.yuanzhike.top

[Q58] 累计求和
来源：http://eux.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aim.andypj.xyz

[Q59] 分组内累计
来源：http://pxj.sufxvd.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gyk.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://bra.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pou.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vdl.ivvv.top


<!-- 参考信息 -->