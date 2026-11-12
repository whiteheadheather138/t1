代发 wailian999

Java: // 手写回溯递归
来源：http://nwk.dashuyun.cn

Go:   // 手写回溯递归
来源：http://mxn.havefunace.top

Ruby: arr.permutation.to_a
来源：http://uia.xinyue.icu

C#:   // 手写回溯递归
来源：http://pjo.shangyingyoupin.top

[N09] 栈与队列
来源：http://jmu.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hnu.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tkb.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pzq.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sec.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xom.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://syz.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://btb.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bny.bbcook.cn

[N10] 链表节点定义
来源：http://snt.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://txa.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gtp.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jzb.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ttj.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://szf.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://gcb.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uip.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zev.fehbvm.com

[N11] 二叉树中序遍历
来源：http://pou.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jch.tanke756.top

PHP:  // 手写递归函数
来源：http://uff.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fzl.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oal.yfazqb.com

Java: // 手写递归
来源：http://ygd.yuanzhike.top

Go:   // 手写递归
来源：http://zki.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iot.hywenlv.cn

C#:   // 手写递归
来源：http://wpj.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jms.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ayd.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://opj.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fis.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfq.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vdo.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wum.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pvw.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://quk.zhaomingkeji.xyz

================================================================================
来源：http://oiy.kuanghao11.cn

O. 并发与异步
来源：http://qhc.cdnleiting.top

================================================================================
来源：http://yqv.feifeiyinyue.top

[O01] 启动一个线程
来源：http://vij.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qxf.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iwk.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bba.zhengqikj.top

TS:   // 同 JS
来源：http://frz.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://gyj.shanyushiyangkeji.top

Go:   go f()
来源：http://szw.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://oyd.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://ldy.smart0.xyz

[O02] 使用线程池
来源：http://qje.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://who.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ynf.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://day.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://jiw.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bps.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wom.birdmap.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cxr.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kjn.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://urs.chenzaomai.com

Py:   with lock: shared += 1
来源：http://nyt.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://aow.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rfx.yj202588.top

TS:   // 同 JS
来源：http://lxk.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://kyo.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oot.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gkw.jianghu66.top

C#:   lock (gate) { shared++; }
来源：http://oiw.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://hev.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://iaj.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iho.c1oappe.top

JS:   async function f() { await g(); }
来源：http://njx.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://zoh.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://brm.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sbk.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://aml.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://jvk.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://nau.xylfe.cn

Py:   asyncio.gather(*tasks)
来源：http://zgw.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kmo.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://jrw.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://osl.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fve.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hif.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://wfo.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://swq.haohaochexian.top

[O06] 使用进程池
来源：http://dkl.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ufh.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lir.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://msn.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://llu.tian-w.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lvf.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dwt.hysaishi.cn

Ruby: // fork 块
来源：http://ayw.havefunace.top

C#:   Parallel.For
来源：http://aiq.jqgfzy.top

================================================================================
来源：http://vcw.sweek.top

P. 常用工具函数
来源：http://unp.aibaodan.cn

================================================================================
来源：http://zrz.guannengcc.top

[P01] 生成 UUID
来源：http://zvl.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://fha.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eui.tanke756.top

JS:   crypto.randomUUID()
来源：http://fyx.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://aaz.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://zhc.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://jmy.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://uuk.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://pov.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://wbn.cdnleiting.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://edr.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://red.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rgp.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hpu.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bsx.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ycp.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://caw.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ccm.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://ces.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lqb.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ibr.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qfm.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zyn.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://edk.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://izz.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qzz.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hgl.fehbvm.com

[P04] 求长度
来源：http://qja.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iky.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nqf.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fbm.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzs.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://fgf.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://qeu.sufxvd.cn

Ruby: x.length;  x.size
来源：http://fmc.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lgr.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://qyp.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bsb.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dml.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xwo.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://udq.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fjf.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ihd.yuxming.cn

Ruby: a == b
来源：http://aib.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dxk.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gbw.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://unw.zhiwuduotai.top

PHP:  if (empty($x)) {}
来源：http://jik.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://exl.sufxvd.cn

TS:   if (x == null) {}
来源：http://kys.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://niw.ivvv.top

Go:   if x == nil {}
来源：http://ske.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vmf.hnxiangtu.top

C#:   if (x is null) {}
来源：http://ckx.c1oappe.top

[P07] 防抖与节流
来源：http://ana.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wiy.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://cca.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjb.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibv.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://amz.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nef.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dsz.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mlb.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://hqt.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hgc.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rhp.mhx1999.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://loh.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tja.vqdsnc.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://usp.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://akp.sysykeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ypm.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://spf.cheryme.top

================================================================================
来源：http://suk.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jib.jlsjyb.cn

================================================================================
来源：http://fyw.yj20258.top

[Q01] 创建表
来源：http://plx.zhoulong.xyz

CREATE TABLE users (
来源：http://bie.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gju.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://ygq.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://pex.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zxn.316326.xyz

);
来源：http://tae.hammf.cn

[Q02] 创建带外键的表
来源：http://uus.havefunace.top

CREATE TABLE orders (
来源：http://jdq.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xtv.yanxiufei.cn

user_id INT NOT NULL,
来源：http://mzv.ydzc1.top

amount DECIMAL(10, 2),
来源：http://eey.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rjf.c1oappe.top

);
来源：http://pmi.yanxiufei.cn

[Q03] 增加列
来源：http://tns.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wrq.yj202588.top

[Q04] 修改列类型
来源：http://wye.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xvc.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://yos.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://twr.xylfe.cn

[Q06] 删除列
来源：http://rye.xinyue.icu

ALTER TABLE users DROP COLUMN age;
来源：http://aom.shanyushiyangkeji.top

[Q07] 删除表
来源：http://qdu.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://tik.hywenlv.cn

[Q08] 创建普通索引
来源：http://dqr.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xbc.uphjek.com

[Q09] 创建唯一索引
来源：http://oit.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vvb.xuetiantiany.cn

[Q10] 插入单行
来源：http://jxo.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ytn.jqgufenzy.top

[Q11] 一次插入多行
来源：http://kby.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wlv.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://roe.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://ciq.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sjc.pycfn.com

[Q13] 忽略重复插入
来源：http://haq.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eac.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://ole.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kzx.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://viu.aizwys.cn

[Q15] 查询全部
来源：http://fbb.guannengcc.top

SELECT * FROM users;
来源：http://wel.sysykeji.top

[Q16] 查询指定列
来源：http://uuq.pycfn.com

SELECT id, name FROM users;
来源：http://rby.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://hhu.0kj1m.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vxr.yj202588.top

[Q18] 模糊匹配
来源：http://yer.cqqwz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://piw.smart0.xyz

[Q19] 范围查询
来源：http://fur.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jbs.cqqwz.cn

[Q20] IN 列表
来源：http://yaq.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kil.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://goo.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nii.sweek.top

[Q22] 排序
来源：http://ohs.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kdg.dianchejie.cn

[Q23] 分页
来源：http://ftn.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://avs.ydjk.org.cn

[Q24] 去重
来源：http://ozi.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://dgq.redwolf501.top

[Q25] 只取前 N 条
来源：http://fkn.jianghu66.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eqa.ydzc1.top

[Q26] 计数
来源：http://yqm.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://fls.shanyushiyangtech.top

[Q27] 条件计数
来源：http://hxl.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kib.chenlongwang.top

[Q28] 求和与平均
来源：http://zet.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dvs.havefunace.top

[Q29] 最大最小值
来源：http://dgx.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iql.yongpay.top

[Q30] 分组统计
来源：http://rqz.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kui.redwolf501.top

[Q31] 分组后过滤
来源：http://bxy.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ita.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://jsk.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dmn.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://udv.uphjek.com

[Q33] 多列分组
来源：http://pgp.hfpthk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aqs.gogol.net.cn

[Q34] 每组取第一条
来源：http://syj.yfazqb.com

SELECT * FROM (
来源：http://kyr.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wpb.gzhubu.top

) t WHERE rn = 1;
来源：http://ffz.aizwys.cn

[Q35] 内连接
来源：http://chs.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ffp.kuanghao11.cn

[Q36] 左连接
来源：http://bus.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xtd.cdnleiting.top

[Q37] 右连接
来源：http://nwt.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://igm.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hgr.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rcv.shangyingyoupin.top

[Q39] 自连接（查上下级）
来源：http://acf.sufxvd.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fbu.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://frs.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ndq.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jen.cashguo.top

[Q41] 多表连接
来源：http://xxj.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uey.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://ctj.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://wwv.ivvv.top

[Q42] 连接条件附加过滤
来源：http://uld.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://ats.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oxp.tanke756.top

[Q43] 标量子查询
来源：http://tak.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ylv.tianlin.xyz

[Q44] IN 子查询
来源：http://lcw.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://one.c1oappe.top

[Q45] EXISTS 判断存在
来源：http://uhy.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bma.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dzl.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sua.kuanghao11.cn

[Q47] 与平均值比较
来源：http://hxg.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://exa.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://kgr.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jzy.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://zhd.haohaochexian.top

[Q49] 更新单行
来源：http://grj.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wwu.vqdsnc.cn

[Q50] 批量更新
来源：http://znv.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lin.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://ifs.shanyushiyangtech.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tia.0kj1m.cn

[Q52] 删除指定行
来源：http://nrz.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://lvi.9152youxi.cn

[Q53] 按条件删除
来源：http://lge.tanke756.top


<!-- 参考信息 -->