代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qvo.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fzi.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mlj.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tiq.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zox.dianchejie.cn

[N10] 链表节点定义
来源：http://dkv.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gra.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://krr.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wct.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qij.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://xbd.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://yyw.yuanzhike.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zbb.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bes.bjfxy.top

[N11] 二叉树中序遍历
来源：http://jyx.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wxo.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://hzu.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gop.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pen.shangyingyoupin.top

Java: // 手写递归
来源：http://tin.fehbvm.com

Go:   // 手写递归
来源：http://dmb.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://irj.fehbvm.com

C#:   // 手写递归
来源：http://klh.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hzx.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ouz.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qkg.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pck.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://evq.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://svo.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://axk.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kde.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ilc.nanxinkj.top

================================================================================
来源：http://ofk.aizwys.cn

O. 并发与异步
来源：http://dmz.c1oappe.top

================================================================================
来源：http://gan.zhixingplan.top

[O01] 启动一个线程
来源：http://uut.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jvj.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nry.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bzq.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://sle.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://kpi.gogol.net.cn

Go:   go f()
来源：http://zqh.shzxlz.cn

Ruby: Thread.new { f }
来源：http://nbt.redwolf501.top

C#:   Task.Run(() => F());
来源：http://dxp.feifeiyinyue.top

[O02] 使用线程池
来源：http://ula.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dgb.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eff.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://nuf.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://fkq.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vln.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://myr.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yfq.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://shv.aizwys.cn

[O03] 加锁保护共享数据
来源：http://csl.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://sym.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://oey.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://etj.chenlongwang.top

TS:   // 同 JS
来源：http://hap.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://tjt.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://thb.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://apn.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://xts.guannengcc.top

[O04] 定义异步函数并等待
来源：http://kmu.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://yuj.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://joi.redwolf501.top

JS:   async function f() { await g(); }
来源：http://xpu.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yqa.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jvo.bbcook.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://peg.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kiq.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://udj.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://cdc.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://wln.hnqzz.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fys.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://kul.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://ebz.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rrs.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jba.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://clw.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wnb.gaohongyu789.top

[O06] 使用进程池
来源：http://ryr.chenlongwang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xvk.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rge.tanke756.top

JS:   // child_process / cluster 模块
来源：http://qbj.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://ard.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wbr.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bvv.shanyushiyangtech.top

Ruby: // fork 块
来源：http://nes.bbcook.cn

C#:   Parallel.For
来源：http://cyl.yuxming.cn

================================================================================
来源：http://blo.ybcxt.top

P. 常用工具函数
来源：http://lbw.gotoacloud.top

================================================================================
来源：http://muq.snrcjt.cn

[P01] 生成 UUID
来源：http://yxu.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://zfa.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kwq.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://yut.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://uyw.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://lww.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://utf.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://pcn.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://wbs.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://ljr.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vyf.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sfe.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://exf.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hkb.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ffe.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qst.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qxb.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://the.hesvh.cn

[P03] 生成短随机字符串
来源：http://wsd.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nlu.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xol.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tal.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uir.fanxiaobao.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hed.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zyf.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nno.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://urz.vehdjk.com

[P04] 求长度
来源：http://gox.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://npk.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dfg.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wlh.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rvu.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://ija.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://qjc.gogol.net.cn

Ruby: x.length;  x.size
来源：http://nly.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xlw.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://ikd.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dsr.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yae.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mon.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sha.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ljj.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://qeu.zhaomingkeji.xyz

Ruby: a == b
来源：http://jae.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lru.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qdf.hywenlv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://seh.yongpay.top

PHP:  if (empty($x)) {}
来源：http://qcn.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xuf.316326.xyz

TS:   if (x == null) {}
来源：http://cxk.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://osj.ehwqpu.com

Go:   if x == nil {}
来源：http://arq.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bzh.vqdsnc.cn

C#:   if (x is null) {}
来源：http://ybs.zhoulong.xyz

[P07] 防抖与节流
来源：http://tsw.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dzv.ivvv.top

PHP:  // 手写时间戳比较
来源：http://cgq.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghr.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pgs.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ehx.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vea.yvedp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://poo.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iuy.xylfe.cn

[P08] 处理浮点精度问题
来源：http://qst.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://awo.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dof.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dcl.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xmu.xziqi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dcw.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jdt.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bpc.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://epj.nwbrower.top

================================================================================
来源：http://ldq.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iqp.daxiang520.top

================================================================================
来源：http://ahl.sjlbkw.cn

[Q01] 创建表
来源：http://tcb.fanxiaobao.xyz

CREATE TABLE users (
来源：http://hcp.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nrt.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://zwr.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://kgv.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cvx.quarkkingdee.top

);
来源：http://rms.andypj.xyz

[Q02] 创建带外键的表
来源：http://jra.zhongyouzk.top

CREATE TABLE orders (
来源：http://brv.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gog.hnqzz.top

user_id INT NOT NULL,
来源：http://emz.tanke756.top

amount DECIMAL(10, 2),
来源：http://svl.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wqk.zhongyouzk.top

);
来源：http://uva.zdbjq.cn

[Q03] 增加列
来源：http://bqo.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kum.sweek.top

[Q04] 修改列类型
来源：http://wkc.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://llo.tianlin.xyz

[Q05] 重命名列
来源：http://ivm.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lam.zhengqikj.top

[Q06] 删除列
来源：http://ffi.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://xjf.yongpay.top

[Q07] 删除表
来源：http://zyw.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://koz.ehwqpu.com

[Q08] 创建普通索引
来源：http://xal.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ble.zdqjudy.top

[Q09] 创建唯一索引
来源：http://lhp.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ttw.yanxiufei.cn

[Q10] 插入单行
来源：http://jmc.fehbvm.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lih.fktsv.cn

[Q11] 一次插入多行
来源：http://epq.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fnj.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://wep.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://tpv.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xzi.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://owr.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://trv.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://cam.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hpd.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ikr.shuidangran.top

[Q15] 查询全部
来源：http://fan.chenjidiqi.icu

SELECT * FROM users;
来源：http://tja.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://fay.sjlbkw.cn

SELECT id, name FROM users;
来源：http://ptq.jinqigufen.top

[Q17] 条件查询
来源：http://jtf.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://snr.zhijiandao.cn

[Q18] 模糊匹配
来源：http://byy.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uuo.yj202588.top

[Q19] 范围查询
来源：http://eqf.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pfm.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://tns.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://orl.ehwqpu.com

[Q21] 空值判断
来源：http://qhr.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ysg.jyoumei.cn

[Q22] 排序
来源：http://byq.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sut.yanxiufei.cn

[Q23] 分页
来源：http://dvx.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tkn.xziqi.cn

[Q24] 去重
来源：http://vdh.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://xap.ivvv.top

[Q25] 只取前 N 条
来源：http://ezu.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nid.chenjidiqi.icu

[Q26] 计数
来源：http://die.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://fyh.wangshuangyany.cn

[Q27] 条件计数
来源：http://ihy.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qkz.shangyingyoupin.top

[Q28] 求和与平均
来源：http://dui.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vdc.cdnleiting.top

[Q29] 最大最小值
来源：http://dvc.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://ain.fzhhl.top

[Q30] 分组统计
来源：http://eni.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lrt.nanxuanxn.top

[Q31] 分组后过滤
来源：http://kgv.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wvw.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://qsq.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xsi.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://btb.fktsv.cn

[Q33] 多列分组
来源：http://vne.sweek.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hmh.xziqi.cn

[Q34] 每组取第一条
来源：http://wqk.sysykeji.top

SELECT * FROM (
来源：http://uis.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lnm.jqgfzy.top

) t WHERE rn = 1;
来源：http://cpm.xziqi.cn

[Q35] 内连接
来源：http://wqg.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pjd.jianghu66.top

[Q36] 左连接
来源：http://mqw.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xwk.vqdsnc.cn

[Q37] 右连接
来源：http://wpc.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wui.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://xdq.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mrs.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://das.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://eld.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qud.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://xjh.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://haj.andypj.xyz

[Q41] 多表连接
来源：http://tzp.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tzs.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://xms.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ubq.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://iwl.yfazqb.com

SELECT u.name, o.amount FROM users u
来源：http://qnx.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://msk.jyoumei.cn

[Q43] 标量子查询
来源：http://vug.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://svy.zdbjq.cn

[Q44] IN 子查询
来源：http://uza.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gcy.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://hok.9152youxi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cqb.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ozy.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uay.tarul.cn

[Q47] 与平均值比较
来源：http://zsn.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://grz.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://rej.cashguo.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ihg.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://bvn.fehbvm.com

[Q49] 更新单行
来源：http://wtk.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fdv.nanxinkj.top

[Q50] 批量更新
来源：http://iov.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://arc.sjlbkw.cn

[Q51] 用子查询更新
来源：http://omf.guannengcc.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://smv.tianlin.xyz

[Q52] 删除指定行
来源：http://whm.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://tee.jqgufenzy.top

[Q53] 按条件删除
来源：http://pkg.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eiu.ydzc1.top

[Q54] 清空表
来源：http://eyw.ybcxt.top

TRUNCATE TABLE logs;
来源：http://czl.yfazqb.com

[Q55] 排名（并列占位）
来源：http://yfx.ydjk.org.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gtn.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://mfg.ywan-chungtsiang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cgo.shzxlz.cn

[Q57] 行号
来源：http://wof.wangshuangyany.cn


<!-- 参考信息 -->