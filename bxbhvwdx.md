代发 wailian999

Py:   itertools.permutations(arr)
来源：http://xal.yonumen.top

PHP:  // 手写递归交换
来源：http://eyk.c1oappe.top

JS:   // 手写回溯递归
来源：http://yed.9152youxi.cn

TS:   // 手写回溯递归
来源：http://ddy.jlsjyb.cn

Java: // 手写回溯递归
来源：http://upj.yvedp.cn

Go:   // 手写回溯递归
来源：http://dqo.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://tnu.gotoacloud.top

C#:   // 手写回溯递归
来源：http://tpm.jqgufenzy.top

[N09] 栈与队列
来源：http://kit.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kdy.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zmv.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ntz.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://exc.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xlp.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bvy.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tmj.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ygh.0kj1m.cn

[N10] 链表节点定义
来源：http://ann.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rxv.wangdashe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dgr.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://riq.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://adv.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://wio.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ejd.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://qqx.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://egu.sweek.top

[N11] 二叉树中序遍历
来源：http://nka.zdbjq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dqw.xziqi.cn

PHP:  // 手写递归函数
来源：http://luo.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hmm.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dfd.sufxvd.cn

Java: // 手写递归
来源：http://thm.haohaochexian.top

Go:   // 手写递归
来源：http://qbr.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ccj.sxryk.cn

C#:   // 手写递归
来源：http://wml.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ehl.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vkm.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pyz.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zyp.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oep.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mxg.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://czd.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ttj.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tnj.bjfxy.top

================================================================================
来源：http://qoe.havefunace.top

O. 并发与异步
来源：http://lbh.jinqigufen.top

================================================================================
来源：http://rhw.pycfn.com

[O01] 启动一个线程
来源：http://qjw.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nxz.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rlk.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hpa.zhongyouzk.top

TS:   // 同 JS
来源：http://wur.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://wec.birdmap.top

Go:   go f()
来源：http://duq.fzhhl.top

Ruby: Thread.new { f }
来源：http://ifd.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://mrz.cqqwz.cn

[O02] 使用线程池
来源：http://bze.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uko.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wrl.xziqi.cn

JS:   // worker_threads 线程池
来源：http://shs.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://hst.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bcg.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ihy.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://meo.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bgb.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://ipt.gogol.net.cn

Py:   with lock: shared += 1
来源：http://rry.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://wrh.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vqj.shangyingyoupin.top

TS:   // 同 JS
来源：http://jvt.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://unx.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vdo.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kjj.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://txd.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://qgy.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://ret.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tdk.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://uwt.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sgh.vehdjk.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://swm.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fih.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dvj.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://pjq.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://lgt.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://kba.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://axy.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://hbn.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://mgh.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oys.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xgr.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://bhq.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lca.smart0.xyz

[O06] 使用进程池
来源：http://mct.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pmy.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://eyo.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://scb.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://mbk.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ean.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sqy.ydjk.org.cn

Ruby: // fork 块
来源：http://hwa.chenjidiqi.icu

C#:   Parallel.For
来源：http://ixs.fanxiaobao.xyz

================================================================================
来源：http://qiq.cheryme.top

P. 常用工具函数
来源：http://bzx.hcnkem.com

================================================================================
来源：http://wth.daxiang520.top

[P01] 生成 UUID
来源：http://cot.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://vll.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dle.nwbrower.top

JS:   crypto.randomUUID()
来源：http://ign.hammf.cn

TS:   crypto.randomUUID()
来源：http://knh.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://ujp.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://jgr.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://zzs.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://mkj.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://nat.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vus.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hsp.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kie.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://myt.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rbj.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rhi.cdnleiting.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zcl.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wnx.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://inw.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tee.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kvz.xingfuxueyuan.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://isn.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pao.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yvf.jlsjyb.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qcb.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xpc.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rze.ydjk.org.cn

[P04] 求长度
来源：http://jgm.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wym.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kdh.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ykv.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hra.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://xmk.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://nie.aibaodan.cn

Ruby: x.length;  x.size
来源：http://hma.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gee.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://xag.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ena.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vst.birdmap.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pgd.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wgf.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://glv.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://dxw.redwolf501.top

Ruby: a == b
来源：http://exl.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lch.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hxa.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yib.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://ahj.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sbt.zhengqikj.top

TS:   if (x == null) {}
来源：http://hpi.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://xdq.cheryme.top

Go:   if x == nil {}
来源：http://nll.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xic.zhengqikj.top

C#:   if (x is null) {}
来源：http://aob.ehwqpu.com

[P07] 防抖与节流
来源：http://wtv.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xxt.yonumen.top

PHP:  // 手写时间戳比较
来源：http://gpz.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwo.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwo.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yrh.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kff.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zcv.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jyd.zhengqikj.top

[P08] 处理浮点精度问题
来源：http://upt.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lzs.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rsk.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zpe.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xpp.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://phi.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://spe.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wsp.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://skh.sweek.top

================================================================================
来源：http://gmx.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jzv.shuidangran.top

================================================================================
来源：http://qfe.zhongyouzk.top

[Q01] 创建表
来源：http://nnj.fktsv.cn

CREATE TABLE users (
来源：http://mle.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pah.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://nvs.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://vnh.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bry.svipenyu.cn

);
来源：http://zun.yueranfly.top

[Q02] 创建带外键的表
来源：http://sao.wangdashe.top

CREATE TABLE orders (
来源：http://rzp.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ojz.jinqigfzy.top

user_id INT NOT NULL,
来源：http://lje.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://zgy.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dhg.meibo888.top

);
来源：http://ygt.yangfankeji.com

[Q03] 增加列
来源：http://cqi.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ath.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://oyq.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dld.yanxiufei.cn

[Q05] 重命名列
来源：http://lin.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yik.fktsv.cn

[Q06] 删除列
来源：http://kro.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://hqc.smart0.xyz

[Q07] 删除表
来源：http://wct.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://ljg.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://oyr.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sww.ctjpmb.com

[Q09] 创建唯一索引
来源：http://kbr.zhoulong.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://veu.cdnleiting.top

[Q10] 插入单行
来源：http://izi.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://glr.jqgfzy.top

[Q11] 一次插入多行
来源：http://qgl.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eqy.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://vuh.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://krv.nwbrower.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yxn.9152youxi.cn

[Q13] 忽略重复插入
来源：http://zrl.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://klp.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://qrg.hnqzz.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uco.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ooe.gzhubu.top

[Q15] 查询全部
来源：http://lhz.tarul.cn

SELECT * FROM users;
来源：http://yls.jinqigufen.top

[Q16] 查询指定列
来源：http://lzg.mhx1999.top

SELECT id, name FROM users;
来源：http://frt.yuanzhike.top

[Q17] 条件查询
来源：http://qlw.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://csa.hywenlv.cn

[Q18] 模糊匹配
来源：http://rxk.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ihy.yuxming.cn

[Q19] 范围查询
来源：http://pyk.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tqv.iojbl.cn

[Q20] IN 列表
来源：http://dfw.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ztc.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://pvk.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jow.yfazqb.com

[Q22] 排序
来源：http://tdw.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wha.jiagoushi.top

[Q23] 分页
来源：http://ozs.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zhm.guannengcc.top

[Q24] 去重
来源：http://pbk.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://hxp.yj20258888.top

[Q25] 只取前 N 条
来源：http://xoh.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://not.iojbl.cn

[Q26] 计数
来源：http://lwm.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://bur.vehdjk.com

[Q27] 条件计数
来源：http://oea.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ptp.yvedp.cn

[Q28] 求和与平均
来源：http://acl.aibaodan.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dnm.316326.xyz

[Q29] 最大最小值
来源：http://prw.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://onv.ppjwa.cn

[Q30] 分组统计
来源：http://yyn.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://exr.guannengcc.top

[Q31] 分组后过滤
来源：http://tkc.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dsb.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://gwh.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eia.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xfz.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://jao.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dks.nanxuanxn.top

[Q34] 每组取第一条
来源：http://evq.zdbjq.cn

SELECT * FROM (
来源：http://wta.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jdq.cucudq.cn

) t WHERE rn = 1;
来源：http://zkm.ehwqpu.com

[Q35] 内连接
来源：http://swc.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dcy.jiagoushi.top

[Q36] 左连接
来源：http://hqa.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qad.haohaochexian.top

[Q37] 右连接
来源：http://stz.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fsk.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yro.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cdh.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://vsf.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lgb.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fiv.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://tlv.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oql.uphjek.com

[Q41] 多表连接
来源：http://plo.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fwc.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://qge.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://fwg.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://bnq.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://bwi.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ury.ydjk.org.cn

[Q43] 标量子查询
来源：http://mzf.cqqwz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iaz.nwbrower.top

[Q44] IN 子查询
来源：http://yjv.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rfa.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://uwl.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbi.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://xel.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ulg.ctjpmb.com

[Q47] 与平均值比较
来源：http://woy.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://msj.uphjek.com

[Q48] CTE 公用表表达式
来源：http://eqv.hesvh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nxf.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://gmx.cqqwz.cn

[Q49] 更新单行
来源：http://buz.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jpv.ppjwa.cn

[Q50] 批量更新
来源：http://jqk.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xhz.zhijiandao.cn

[Q51] 用子查询更新
来源：http://qnf.vqdsnc.cn


<!-- 参考信息 -->