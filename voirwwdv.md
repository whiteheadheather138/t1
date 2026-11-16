代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ltc.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wqf.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bnm.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sfs.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sdn.zhixingplan.top

[N10] 链表节点定义
来源：http://cwf.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ryg.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wqz.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yrq.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://afj.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://dvu.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://net.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jat.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hak.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://ael.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uis.vehdjk.com

PHP:  // 手写递归函数
来源：http://jza.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xat.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blm.zhoulong.xyz

Java: // 手写递归
来源：http://dpj.shangyingyoupin.top

Go:   // 手写递归
来源：http://qzo.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oih.havefunace.top

C#:   // 手写递归
来源：http://oba.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kqh.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://itk.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://djy.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vfy.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nvn.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sod.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aqa.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jcr.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wxt.shangyingyoupin.top

================================================================================
来源：http://mto.gaohongyu789.top

O. 并发与异步
来源：http://kfy.ehwqpu.com

================================================================================
来源：http://raq.zdqjudy.top

[O01] 启动一个线程
来源：http://hsc.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zjf.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ijy.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wdr.pycfn.com

TS:   // 同 JS
来源：http://iuy.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://ljg.yfazqb.com

Go:   go f()
来源：http://aqn.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://niy.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://eha.havefunace.top

[O02] 使用线程池
来源：http://mdc.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lwe.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yyd.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://zrc.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://fkm.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://hvc.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qrj.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wuh.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pme.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://xay.tanke756.top

Py:   with lock: shared += 1
来源：http://poq.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://vae.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qvn.daria6918.cn

TS:   // 同 JS
来源：http://ljj.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://eqm.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ude.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ked.sweek.top

C#:   lock (gate) { shared++; }
来源：http://zvn.52xcode.cn

[O04] 定义异步函数并等待
来源：http://vid.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://vgf.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ewm.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://luk.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yyb.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eie.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wbj.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dum.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://zrr.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://xao.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://bci.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lvm.meibo888.top

JS:   await Promise.all(tasks)
来源：http://ftt.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://wky.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lrp.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dsf.birdmap.top

Ruby: threads.map(&:join)
来源：http://pdj.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fni.aizwys.cn

[O06] 使用进程池
来源：http://udr.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jcs.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://ege.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://atj.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://vzk.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nic.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uxw.hnxiangtu.top

Ruby: // fork 块
来源：http://ikg.ydzc1.top

C#:   Parallel.For
来源：http://auq.sjlbkw.cn

================================================================================
来源：http://cyl.c1oappe.top

P. 常用工具函数
来源：http://vhh.zdbjq.cn

================================================================================
来源：http://ibd.jqgufenzy.top

[P01] 生成 UUID
来源：http://ehb.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://lye.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gts.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://fyk.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://wzq.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://vyr.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://ncf.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://grb.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://thh.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://qwl.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vkv.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oai.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sja.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sfh.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xkt.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oai.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bwu.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://etb.cdnleiting.top

[P03] 生成短随机字符串
来源：http://bij.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bdn.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ehs.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nup.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bct.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wkc.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fmy.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pac.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://awg.kuanghao11.cn

[P04] 求长度
来源：http://urp.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jtq.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oss.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bmw.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dzt.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://plt.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://dil.316326.xyz

Ruby: x.length;  x.size
来源：http://kny.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zyv.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://ygl.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nmg.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kcp.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wwc.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dvm.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fja.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://xiq.bjfxy.top

Ruby: a == b
来源：http://ckb.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gen.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lld.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jul.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://dab.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vfe.fzhhl.top

TS:   if (x == null) {}
来源：http://rzu.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qqw.ehwqpu.com

Go:   if x == nil {}
来源：http://fcx.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mgx.xziqi.cn

C#:   if (x is null) {}
来源：http://sfm.feifeiyinyue.top

[P07] 防抖与节流
来源：http://nty.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kdy.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://sbl.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbw.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xay.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lzi.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rol.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mrz.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cse.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://vze.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://obp.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gkp.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tke.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://alh.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://utq.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vjb.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zoj.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://atl.tarul.cn

================================================================================
来源：http://bvl.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gzy.sweek.top

================================================================================
来源：http://hys.gotoacloud.top

[Q01] 创建表
来源：http://vhs.xziqi.cn

CREATE TABLE users (
来源：http://jmq.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://huv.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://pnu.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://ibo.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tla.ivvv.top

);
来源：http://eqa.tian-w.cn

[Q02] 创建带外键的表
来源：http://ryg.svipenyu.cn

CREATE TABLE orders (
来源：http://fej.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://klu.yj20258.top

user_id INT NOT NULL,
来源：http://nrk.smart0.xyz

amount DECIMAL(10, 2),
来源：http://kbj.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oft.yongpay.top

);
来源：http://iln.kuanghao11.cn

[Q03] 增加列
来源：http://uhx.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tcz.0kj1m.cn

[Q04] 修改列类型
来源：http://ykj.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hfj.gotoacloud.top

[Q05] 重命名列
来源：http://ylk.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xzy.fehbvm.com

[Q06] 删除列
来源：http://bqc.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://ciy.sysykeji.top

[Q07] 删除表
来源：http://ydz.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://wjw.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://ekp.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://psn.aizwys.cn

[Q09] 创建唯一索引
来源：http://uhg.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fyr.fengsongda.top

[Q10] 插入单行
来源：http://ara.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cwh.tianlin.xyz

[Q11] 一次插入多行
来源：http://mbc.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ixt.havefunace.top

[Q12] 插入后取自增 ID
来源：http://nqc.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://riy.ydjk.org.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wfz.shuidangran.top

[Q13] 忽略重复插入
来源：http://wfp.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ahd.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://rqm.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oto.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://noh.sysykeji.top

[Q15] 查询全部
来源：http://xce.hnxiangtu.top

SELECT * FROM users;
来源：http://zwi.zdbjq.cn

[Q16] 查询指定列
来源：http://gmp.sxryk.cn

SELECT id, name FROM users;
来源：http://bdm.zhongyouzk.top

[Q17] 条件查询
来源：http://sfs.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vyb.hfpthk.cn

[Q18] 模糊匹配
来源：http://cjm.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pzo.smart0.xyz

[Q19] 范围查询
来源：http://ifc.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lmj.jiagoushi.top

[Q20] IN 列表
来源：http://kcp.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dor.sufxvd.cn

[Q21] 空值判断
来源：http://iax.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rkw.gotoacloud.top

[Q22] 排序
来源：http://lmo.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cfr.redwolf501.top

[Q23] 分页
来源：http://dbo.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tpo.daria6918.cn

[Q24] 去重
来源：http://rgo.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://vly.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://gbo.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://obb.ivvv.top

[Q26] 计数
来源：http://vdk.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://utw.dashuyun.cn

[Q27] 条件计数
来源：http://ndc.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://skd.gotoacloud.top

[Q28] 求和与平均
来源：http://ikz.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zgi.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://fyy.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ssk.zdqjudy.top

[Q30] 分组统计
来源：http://zye.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://suq.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://any.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zah.tian-w.cn

[Q32] 分组拼接字符串
来源：http://qbo.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jxf.yangfankeji.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bts.birdmap.top

[Q33] 多列分组
来源：http://xro.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hlt.kuanghao11.cn

[Q34] 每组取第一条
来源：http://ggq.hongshengwenyu.top

SELECT * FROM (
来源：http://yjv.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xrp.yuanzhike.top

) t WHERE rn = 1;
来源：http://edj.meibo888.top

[Q35] 内连接
来源：http://npn.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sbu.yj20258888.top

[Q36] 左连接
来源：http://znf.xuetiantiany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oge.yj202588.top

[Q37] 右连接
来源：http://cpx.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eex.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pbz.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gct.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://xzw.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xwo.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kyl.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mme.hesvh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fbk.xuanzx.com

[Q41] 多表连接
来源：http://iqt.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hug.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://xyg.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://fuy.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://uuq.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://gmu.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rwy.gaohongyu789.top

[Q43] 标量子查询
来源：http://cgq.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dac.tian-w.cn

[Q44] IN 子查询
来源：http://mix.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tht.havefunace.top

[Q45] EXISTS 判断存在
来源：http://xah.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yhf.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dij.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://byc.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://gll.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jjr.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://ooj.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sdj.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://mrz.vehdjk.com

[Q49] 更新单行
来源：http://njs.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oxf.guowangkeji.top

[Q50] 批量更新
来源：http://uly.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://trh.yueranfly.top

[Q51] 用子查询更新
来源：http://rpm.zhaomingkeji.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ano.52xcode.cn

[Q52] 删除指定行
来源：http://bzc.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://sio.fktsv.cn

[Q53] 按条件删除
来源：http://ayi.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uaq.aizwys.cn

[Q54] 清空表
来源：http://njc.mhx1999.top

TRUNCATE TABLE logs;
来源：http://puo.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://qxm.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rwp.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://gsi.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://esf.jiagoushi.top

[Q57] 行号
来源：http://qln.hongshengwenyu.top


<!-- 参考信息 -->