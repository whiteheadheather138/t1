代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://srt.ctjpmb.com

[N10] 链表节点定义
来源：http://twe.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vvm.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cuc.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ktn.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pjq.yj20258.top

Java: class Node { int v; Node next; }
来源：http://lyg.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://nuq.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://exc.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://kyp.c1oappe.top

[N11] 二叉树中序遍历
来源：http://lnq.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oxr.nanxinkj.top

PHP:  // 手写递归函数
来源：http://yzj.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zpb.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ldk.xinyue.icu

Java: // 手写递归
来源：http://eza.cucudq.cn

Go:   // 手写递归
来源：http://izz.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fev.haohaochexian.top

C#:   // 手写递归
来源：http://zxk.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hsp.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ycb.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://edn.jqgfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kuw.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qca.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wiz.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rdd.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zax.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://byp.wangdashe.top

================================================================================
来源：http://uqb.sysykeji.top

O. 并发与异步
来源：http://bfr.vqdsnc.cn

================================================================================
来源：http://pma.cucudq.cn

[O01] 启动一个线程
来源：http://hmf.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xxd.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uou.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xiy.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://jda.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://qwd.52xcode.cn

Go:   go f()
来源：http://lok.sweek.top

Ruby: Thread.new { f }
来源：http://wgm.xinyue.icu

C#:   Task.Run(() => F());
来源：http://rhj.xziqi.cn

[O02] 使用线程池
来源：http://qvy.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mjz.fzhhl.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oqh.hesvh.cn

JS:   // worker_threads 线程池
来源：http://cho.fzhhl.top

TS:   // worker_threads 线程池
来源：http://piu.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://biz.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tjk.shanyushiyangtech.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vsh.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ckk.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://lfx.snrcjt.cn

Py:   with lock: shared += 1
来源：http://yhq.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://adj.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yfg.ctjpmb.com

TS:   // 同 JS
来源：http://uwh.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://kbx.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gjz.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://grr.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://prk.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://rjo.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://kmc.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lay.ctjpmb.com

JS:   async function f() { await g(); }
来源：http://lyv.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mmx.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yor.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://swd.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ldf.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://sga.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://ssz.epnwcf.com

Py:   asyncio.gather(*tasks)
来源：http://mlh.hnqzz.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cus.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://isy.yj202588.top

TS:   await Promise.all(tasks)
来源：http://zcx.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ndb.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uji.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://mcy.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://kva.chenzaomai.com

[O06] 使用进程池
来源：http://vri.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qgy.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://elb.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://pus.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://azf.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dxs.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rjn.sjlbkw.cn

Ruby: // fork 块
来源：http://avb.aizwys.cn

C#:   Parallel.For
来源：http://avt.hfpthk.cn

================================================================================
来源：http://fzz.yuxming.cn

P. 常用工具函数
来源：http://jfs.mhx1999.top

================================================================================
来源：http://qru.jqgfzy.top

[P01] 生成 UUID
来源：http://ozg.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://cno.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pei.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://bby.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://eww.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://bsx.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://vfl.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://iqo.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://dpg.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://exf.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xvn.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nbt.pycfn.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ftb.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lrk.yfazqb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://heg.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hae.smart0.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vhb.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qxc.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://qir.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://exa.vqdsnc.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qoq.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zyk.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zhk.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sud.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tzf.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xqp.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kpa.hnxiangtu.top

[P04] 求长度
来源：http://idv.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cvq.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wck.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tqk.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eka.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://mfb.jianghu66.top

Go:   len(arr);  len(m)
来源：http://zka.ppjwa.cn

Ruby: x.length;  x.size
来源：http://buo.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://ila.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://yka.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://man.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dmu.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tob.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wus.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mel.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://baa.epnwcf.com

Ruby: a == b
来源：http://ddt.zhiwuduotai.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://twg.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pqm.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kfl.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://udz.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ztv.xuanzx.com

TS:   if (x == null) {}
来源：http://tfb.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zjd.epnwcf.com

Go:   if x == nil {}
来源：http://fkm.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vvv.aizwys.cn

C#:   if (x is null) {}
来源：http://uto.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://qsk.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rwd.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://dge.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vac.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhp.mhx1999.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://guz.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rjv.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ldn.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gbb.xziqi.cn

[P08] 处理浮点精度问题
来源：http://muh.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dmw.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ufh.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://imx.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vsj.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mlc.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lbo.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gfc.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gpg.chenlongwang.top

================================================================================
来源：http://kpv.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://phq.zdqjudy.top

================================================================================
来源：http://prf.ydzc1.top

[Q01] 创建表
来源：http://jpt.shzxlz.cn

CREATE TABLE users (
来源：http://mbk.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bdv.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://jsw.0kj1m.cn

email VARCHAR(100) UNIQUE,
来源：http://jlh.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iml.jqgfzy.top

);
来源：http://nqu.ybcxt.top

[Q02] 创建带外键的表
来源：http://vit.zhoulong.xyz

CREATE TABLE orders (
来源：http://kfe.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yyf.nwbrower.top

user_id INT NOT NULL,
来源：http://dfw.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://mos.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://omr.hysaishi.cn

);
来源：http://uph.zhoulong.xyz

[Q03] 增加列
来源：http://ore.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hpf.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://qdu.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uux.zdqjudy.top

[Q05] 重命名列
来源：http://vhw.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dmo.jyoumei.cn

[Q06] 删除列
来源：http://kgw.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://ejz.chenjidiqi.icu

[Q07] 删除表
来源：http://shy.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://wxf.smart0.xyz

[Q08] 创建普通索引
来源：http://kap.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ihw.tian-w.cn

[Q09] 创建唯一索引
来源：http://nob.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xhs.snrcjt.cn

[Q10] 插入单行
来源：http://neu.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fmc.yj20258888.top

[Q11] 一次插入多行
来源：http://rgk.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://flg.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://oil.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lhw.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ijq.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://rii.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://esu.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://tcz.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uut.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lkx.ehwqpu.com

[Q15] 查询全部
来源：http://nib.cheryme.top

SELECT * FROM users;
来源：http://qhg.birdmap.top

[Q16] 查询指定列
来源：http://bcf.ppjwa.cn

SELECT id, name FROM users;
来源：http://jqe.yj20258.top

[Q17] 条件查询
来源：http://ems.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ekp.iojbl.cn

[Q18] 模糊匹配
来源：http://itz.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bba.guannengcc.top

[Q19] 范围查询
来源：http://uck.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fkn.yj20258888.top

[Q20] IN 列表
来源：http://abp.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://crh.aibaodan.cn

[Q21] 空值判断
来源：http://gud.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nny.aizwys.cn

[Q22] 排序
来源：http://tux.hesvh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oib.fzhhl.top

[Q23] 分页
来源：http://ynm.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://olk.hysaishi.cn

[Q24] 去重
来源：http://eyl.ydjk.org.cn

SELECT DISTINCT city FROM users;
来源：http://cvv.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://rjk.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jtp.jinyuanbaomall.cn

[Q26] 计数
来源：http://qjb.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://bln.jlsjyb.cn

[Q27] 条件计数
来源：http://ekn.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://raf.cashguo.top

[Q28] 求和与平均
来源：http://giw.yj20258888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mgh.jlsjyb.cn

[Q29] 最大最小值
来源：http://vmx.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bkt.c1oappe.top

[Q30] 分组统计
来源：http://xdd.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cds.hcnkem.com

[Q31] 分组后过滤
来源：http://smo.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vqo.yueranfly.top

[Q32] 分组拼接字符串
来源：http://bqj.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qlq.tarul.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gmb.dianchejie.cn

[Q33] 多列分组
来源：http://qul.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ayq.gzhubu.top

[Q34] 每组取第一条
来源：http://yho.redwolf501.top

SELECT * FROM (
来源：http://aym.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cyn.ybcxt.top

) t WHERE rn = 1;
来源：http://smo.cucudq.cn

[Q35] 内连接
来源：http://iir.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://chr.pengpengdd.cyou

[Q36] 左连接
来源：http://voo.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jyb.fehbvm.com

[Q37] 右连接
来源：http://qch.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://emr.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://akk.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qtl.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://oko.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mtp.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eql.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://hlm.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ucp.jlsjyb.cn

[Q41] 多表连接
来源：http://tyr.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://nkc.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://rrl.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://jrx.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://qcd.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://wdv.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ugk.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://xej.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aqp.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://xid.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://atf.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://xbm.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eok.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://pzm.yueranfly.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qok.andypj.xyz

[Q47] 与平均值比较
来源：http://txm.ivvv.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xly.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://oxl.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://boc.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://zsl.ivvv.top

[Q49] 更新单行
来源：http://uha.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hwq.hesvh.cn

[Q50] 批量更新
来源：http://yhu.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pom.daxiang520.top

[Q51] 用子查询更新
来源：http://xzi.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hsn.gotoacloud.top

[Q52] 删除指定行
来源：http://nvm.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://hmc.ppjwa.cn

[Q53] 按条件删除
来源：http://usv.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cvo.aibaodan.cn

[Q54] 清空表
来源：http://qkw.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://utc.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://mci.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zku.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://vhf.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wgw.ybcxt.top

[Q57] 行号
来源：http://fpy.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lgd.tanke756.top

[Q58] 累计求和
来源：http://tuf.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://etg.sufxvd.cn

[Q59] 分组内累计
来源：http://xzf.guowangkeji.top


<!-- 参考信息 -->