代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sov.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jkt.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ajl.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nbg.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://url.chenjidiqi.icu

[N10] 链表节点定义
来源：http://qwe.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ehq.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ffw.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ngi.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jmn.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://mpa.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://edo.jianghu66.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mhf.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://czy.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://jfr.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pqt.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://qxl.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ccx.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bil.zhixingplan.top

Java: // 手写递归
来源：http://rtc.jqgfzy.top

Go:   // 手写递归
来源：http://biv.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hbn.hywenlv.cn

C#:   // 手写递归
来源：http://qsr.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bzd.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://spa.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cck.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wql.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://swc.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yib.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nxe.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hco.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hec.yongpay.top

================================================================================
来源：http://swe.yuanzhike.top

O. 并发与异步
来源：http://cil.bjfxy.top

================================================================================
来源：http://bzb.jianghu66.top

[O01] 启动一个线程
来源：http://upo.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eke.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://znk.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uzh.cucudq.cn

TS:   // 同 JS
来源：http://hkx.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://nwe.iojbl.cn

Go:   go f()
来源：http://obl.ybcxt.top

Ruby: Thread.new { f }
来源：http://dev.xinyue.icu

C#:   Task.Run(() => F());
来源：http://lrd.fanxiaobao.xyz

[O02] 使用线程池
来源：http://rxj.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iph.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vgl.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://wbc.nwbrower.top

TS:   // worker_threads 线程池
来源：http://xvm.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://lqj.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://plp.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nil.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eiq.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://wxh.shzxlz.cn

Py:   with lock: shared += 1
来源：http://igi.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://fpc.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uft.pycfn.com

TS:   // 同 JS
来源：http://lnp.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://skj.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cco.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://otx.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://kxj.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://gpt.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://ueo.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aud.sxryk.cn

JS:   async function f() { await g(); }
来源：http://emq.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ogf.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://utr.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nmc.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://jti.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://fex.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://jaj.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://vsy.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ulq.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://owt.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://twq.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hni.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nai.ybcxt.top

Ruby: threads.map(&:join)
来源：http://jrg.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cax.tarul.cn

[O06] 使用进程池
来源：http://jic.snrcjt.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ysm.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xyo.sxryk.cn

JS:   // child_process / cluster 模块
来源：http://pcy.tanke756.top

TS:   // child_process / cluster 模块
来源：http://rtj.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iqy.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ibq.hongshengwenyu.top

Ruby: // fork 块
来源：http://oag.haohaochexian.top

C#:   Parallel.For
来源：http://nst.ehwqpu.com

================================================================================
来源：http://bnl.yvedp.cn

P. 常用工具函数
来源：http://yjd.gaohongyu789.top

================================================================================
来源：http://vfm.mhx1999.top

[P01] 生成 UUID
来源：http://zee.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://lns.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cjk.zycfv.cn

JS:   crypto.randomUUID()
来源：http://nyd.xinyue.icu

TS:   crypto.randomUUID()
来源：http://nuz.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://bjy.smart0.xyz

Go:   // 用 github.com/google/uuid
来源：http://ggv.yongpay.top

Ruby: SecureRandom.uuid
来源：http://hzt.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://dku.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://eik.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ktd.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ias.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ijv.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vxc.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nko.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://paq.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://swx.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tcw.wangdashe.top

[P03] 生成短随机字符串
来源：http://fqt.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dth.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://udi.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xjo.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bse.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xth.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rgq.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qmi.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wsy.jyoumei.cn

[P04] 求长度
来源：http://nau.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jgp.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dbi.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zwb.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sgm.fehbvm.com

Java: list.size();  map.size();  s.length()
来源：http://llz.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://fzs.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://uoy.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xoe.uphjek.com

[P05] 判断两个对象内容是否相等
来源：http://upy.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qbw.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://reu.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wbb.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ucf.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bal.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://fcs.jyoumei.cn

Ruby: a == b
来源：http://pnr.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gyv.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dmc.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fgs.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://pqj.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zns.jianghu66.top

TS:   if (x == null) {}
来源：http://kbw.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iqw.snrcjt.cn

Go:   if x == nil {}
来源：http://yyx.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fym.316326.xyz

C#:   if (x is null) {}
来源：http://sqi.zhixingplan.top

[P07] 防抖与节流
来源：http://rnp.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zmv.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://ghk.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhu.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yaz.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://axx.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nez.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ink.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fhm.xuanzx.com

[P08] 处理浮点精度问题
来源：http://inb.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bhu.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gnq.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ulz.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sac.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fhv.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xbn.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bet.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ueg.snrcjt.cn

================================================================================
来源：http://cxg.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ler.ivvv.top

================================================================================
来源：http://ush.andypj.xyz

[Q01] 创建表
来源：http://lvp.ppjwa.cn

CREATE TABLE users (
来源：http://bdu.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://snq.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://nru.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://sag.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://chn.zdqjudy.top

);
来源：http://rea.svipenyu.cn

[Q02] 创建带外键的表
来源：http://cpz.chenzaomai.com

CREATE TABLE orders (
来源：http://qqz.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yuy.fengsongda.top

user_id INT NOT NULL,
来源：http://fza.ivvv.top

amount DECIMAL(10, 2),
来源：http://rtu.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hah.chenlongwang.top

);
来源：http://gsy.aizwys.cn

[Q03] 增加列
来源：http://btc.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nci.52xcode.cn

[Q04] 修改列类型
来源：http://tdx.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://det.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://kzu.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vnw.zdqjudy.top

[Q06] 删除列
来源：http://czd.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://mns.sjlbkw.cn

[Q07] 删除表
来源：http://ldi.xylfe.cn

DROP TABLE IF EXISTS orders;
来源：http://txh.hesvh.cn

[Q08] 创建普通索引
来源：http://sqv.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zag.aizwys.cn

[Q09] 创建唯一索引
来源：http://dcr.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nkm.hammf.cn

[Q10] 插入单行
来源：http://ijh.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wwd.zhijiandao.cn

[Q11] 一次插入多行
来源：http://kar.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zvm.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://vct.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://xic.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wkq.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://xos.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wey.sweek.top

[Q14] 存在则更新（upsert）
来源：http://tgz.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qjl.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mbr.jqgufenzy.top

[Q15] 查询全部
来源：http://ail.jinqigufen.top

SELECT * FROM users;
来源：http://oqw.dianchejie.cn

[Q16] 查询指定列
来源：http://pmj.jyoumei.cn

SELECT id, name FROM users;
来源：http://brd.zhijiandao.cn

[Q17] 条件查询
来源：http://bsm.0kj1m.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mcq.yj202588.top

[Q18] 模糊匹配
来源：http://dwx.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iyy.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://xsd.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uxv.chenzaomai.com

[Q20] IN 列表
来源：http://pdk.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bsz.havefunace.top

[Q21] 空值判断
来源：http://cvb.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://wfa.andypj.xyz

[Q22] 排序
来源：http://fkv.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mmg.yongpay.top

[Q23] 分页
来源：http://mnf.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://frt.haohaochexian.top

[Q24] 去重
来源：http://wou.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://wfq.daria6918.cn

[Q25] 只取前 N 条
来源：http://wds.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rkf.pengpengdd.cyou

[Q26] 计数
来源：http://uxc.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://lkg.yj20258888.top

[Q27] 条件计数
来源：http://hoh.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yhy.sufxvd.cn

[Q28] 求和与平均
来源：http://hgm.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jpe.ydjk.org.cn

[Q29] 最大最小值
来源：http://mlx.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://akw.vqdsnc.cn

[Q30] 分组统计
来源：http://ctb.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uyz.gogol.net.cn

[Q31] 分组后过滤
来源：http://wja.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cqz.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://qik.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fnd.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qtu.svipenyu.cn

[Q33] 多列分组
来源：http://oww.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aog.meibo888.top

[Q34] 每组取第一条
来源：http://hyu.yj202588.top

SELECT * FROM (
来源：http://vgj.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dqm.sjlbkw.cn

) t WHERE rn = 1;
来源：http://llc.havefunace.top

[Q35] 内连接
来源：http://mir.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mse.yanxiufei.cn

[Q36] 左连接
来源：http://zbd.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ace.yueranfly.top

[Q37] 右连接
来源：http://lix.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ekc.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://dca.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wlv.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://cta.sufxvd.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rcs.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://adz.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iha.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ast.epnwcf.com

[Q41] 多表连接
来源：http://zor.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tvc.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://pji.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://fwr.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://vqq.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://hzr.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://isd.tanke756.top

[Q43] 标量子查询
来源：http://ogt.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nek.cqqwz.cn

[Q44] IN 子查询
来源：http://htd.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ajo.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://jml.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pso.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://rqy.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uni.xuanzx.com

[Q47] 与平均值比较
来源：http://mll.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://twf.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://glm.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://odi.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://hnz.daria6918.cn

[Q49] 更新单行
来源：http://gbi.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ncj.dianchejie.cn

[Q50] 批量更新
来源：http://abs.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hhp.fehbvm.com

[Q51] 用子查询更新
来源：http://drk.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eax.hesvh.cn

[Q52] 删除指定行
来源：http://enb.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://bze.feifeiyinyue.top

[Q53] 按条件删除
来源：http://zge.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://igx.shuidangran.top

[Q54] 清空表
来源：http://xep.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://edn.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://ker.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://orq.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://mwx.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xaq.ywan-chungtsiang.top

[Q57] 行号
来源：http://qio.zdbjq.cn


<!-- 参考信息 -->