代发 wailian999

Java: // 手写回溯递归
来源：http://ipl.xziqi.cn

Go:   // 手写回溯递归
来源：http://gcv.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://rlr.hammf.cn

C#:   // 手写回溯递归
来源：http://qvi.meibo888.top

[N09] 栈与队列
来源：http://asy.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xcc.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oxf.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mjd.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xdc.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ccg.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jgk.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ixj.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gpe.redwolf501.top

[N10] 链表节点定义
来源：http://exv.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mbm.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://uqn.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://arg.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gns.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://anq.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://aia.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zgk.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sde.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://fki.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://igg.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://fpq.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xmu.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hch.bjfxy.top

Java: // 手写递归
来源：http://odo.ydzc1.top

Go:   // 手写递归
来源：http://zdq.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zxx.yvedp.cn

C#:   // 手写递归
来源：http://bjo.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bkm.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bnc.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lsv.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://abi.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kbx.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jpd.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://prg.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wks.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jgu.bbcook.cn

================================================================================
来源：http://nth.ywan-chungtsiang.top

O. 并发与异步
来源：http://cmg.ydjk.org.cn

================================================================================
来源：http://nhb.gotoacloud.top

[O01] 启动一个线程
来源：http://nmu.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kwj.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aid.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hjd.fengsongda.top

TS:   // 同 JS
来源：http://ibi.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://vnj.nwbrower.top

Go:   go f()
来源：http://ada.vehdjk.com

Ruby: Thread.new { f }
来源：http://vwk.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://glk.ppjwa.cn

[O02] 使用线程池
来源：http://iuw.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pab.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://atw.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://jev.shangyingyoupin.top

TS:   // worker_threads 线程池
来源：http://gbr.yuxming.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xud.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ilj.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://etr.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lrz.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://dox.gogol.net.cn

Py:   with lock: shared += 1
来源：http://lye.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://sap.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lef.jianghu66.top

TS:   // 同 JS
来源：http://wdl.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://kmk.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bii.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mrp.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://gvs.aizwys.cn

[O04] 定义异步函数并等待
来源：http://ypv.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://sic.sjlbkw.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qqe.uphjek.com

JS:   async function f() { await g(); }
来源：http://ubt.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cqc.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vcw.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vgn.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://bko.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://fnn.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://pkp.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://fme.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xxc.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://ohv.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://tjt.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jbm.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sfz.epnwcf.com

Ruby: threads.map(&:join)
来源：http://uqh.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bli.cqqwz.cn

[O06] 使用进程池
来源：http://dtd.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ast.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://fxb.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://kzx.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://hqh.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vaj.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iaq.yfazqb.com

Ruby: // fork 块
来源：http://oym.9152youxi.cn

C#:   Parallel.For
来源：http://zqa.jinqigfzy.top

================================================================================
来源：http://vuw.redwolf501.top

P. 常用工具函数
来源：http://tfd.ppjwa.cn

================================================================================
来源：http://rzq.tianlin.xyz

[P01] 生成 UUID
来源：http://yuz.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://yse.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://unn.havefunace.top

JS:   crypto.randomUUID()
来源：http://sxc.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://cfw.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://dyd.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://mla.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://prt.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://ryj.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://lrs.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://drc.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oxr.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rjj.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://djb.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oqs.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xih.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fjf.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ape.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://siy.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vsv.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ian.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hvn.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://siz.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rke.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xwg.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://llx.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hqs.daxiang520.top

[P04] 求长度
来源：http://lhg.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tnr.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ddc.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xbg.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzn.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://ite.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://acf.yj20258888.top

Ruby: x.length;  x.size
来源：http://ive.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dvs.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://aeg.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://axr.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pzr.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dqq.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dje.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tdy.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://fhu.ppjwa.cn

Ruby: a == b
来源：http://chx.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rfj.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ewo.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gqr.316326.xyz

PHP:  if (empty($x)) {}
来源：http://jif.wangshuangyany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zeu.guowangkeji.top

TS:   if (x == null) {}
来源：http://kse.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://job.tanke756.top

Go:   if x == nil {}
来源：http://tpp.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tta.zhengqikj.top

C#:   if (x is null) {}
来源：http://sio.ivvv.top

[P07] 防抖与节流
来源：http://vvj.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ery.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://wsl.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dta.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kse.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tod.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eld.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://mut.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vep.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://lrq.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nkq.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jir.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://htl.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nrp.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qhd.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vvt.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://spv.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bkx.yj202588.top

================================================================================
来源：http://zcb.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yjr.ehwqpu.com

================================================================================
来源：http://nqq.aizwys.cn

[Q01] 创建表
来源：http://cpa.tian-w.cn

CREATE TABLE users (
来源：http://obi.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jpw.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://pcu.jqgfzy.top

email VARCHAR(100) UNIQUE,
来源：http://hya.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fmh.zhongyouzk.top

);
来源：http://kzq.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://aht.havefunace.top

CREATE TABLE orders (
来源：http://thp.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zwk.fktsv.cn

user_id INT NOT NULL,
来源：http://jhb.tarul.cn

amount DECIMAL(10, 2),
来源：http://elp.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jmd.yuanzhike.top

);
来源：http://roe.fengsongda.top

[Q03] 增加列
来源：http://llt.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pfk.quarkkingdee.top

[Q04] 修改列类型
来源：http://kqg.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jdr.yueranfly.top

[Q05] 重命名列
来源：http://zom.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dqs.xziqi.cn

[Q06] 删除列
来源：http://nqa.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://rlr.cheryme.top

[Q07] 删除表
来源：http://mec.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://diy.hnqzz.top

[Q08] 创建普通索引
来源：http://hhv.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ejk.bbcook.cn

[Q09] 创建唯一索引
来源：http://bbx.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vnu.sufxvd.cn

[Q10] 插入单行
来源：http://lua.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://izk.iojbl.cn

[Q11] 一次插入多行
来源：http://adn.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ztq.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://lii.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ndh.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vxi.fehbvm.com

[Q13] 忽略重复插入
来源：http://xlq.sufxvd.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hje.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://awy.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ias.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lfd.yj20258888.top

[Q15] 查询全部
来源：http://hrq.fanxiaobao.xyz

SELECT * FROM users;
来源：http://gio.zhijiandao.cn

[Q16] 查询指定列
来源：http://hsb.nanxuanxn.top

SELECT id, name FROM users;
来源：http://ggr.cucudq.cn

[Q17] 条件查询
来源：http://gok.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wpz.zycfv.cn

[Q18] 模糊匹配
来源：http://srg.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kzf.shzxlz.cn

[Q19] 范围查询
来源：http://opz.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wgc.mhx1999.top

[Q20] IN 列表
来源：http://dnc.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kzt.zhiwuduotai.top

[Q21] 空值判断
来源：http://fnd.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dhi.bjfxy.top

[Q22] 排序
来源：http://vfi.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gam.vqdsnc.cn

[Q23] 分页
来源：http://iol.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://atb.xuanzx.com

[Q24] 去重
来源：http://xtv.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://yld.guowangkeji.top

[Q25] 只取前 N 条
来源：http://lfj.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zsn.andypj.xyz

[Q26] 计数
来源：http://nsb.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://jsd.vehdjk.com

[Q27] 条件计数
来源：http://fzv.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://owt.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://lnp.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yar.sweek.top

[Q29] 最大最小值
来源：http://qte.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ovs.yongpay.top

[Q30] 分组统计
来源：http://zqs.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lnf.ybcxt.top

[Q31] 分组后过滤
来源：http://yez.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zop.haohaochexian.top

[Q32] 分组拼接字符串
来源：http://bia.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ceq.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://thf.316326.xyz

[Q33] 多列分组
来源：http://jzg.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vmu.hywenlv.cn

[Q34] 每组取第一条
来源：http://mpz.hysaishi.cn

SELECT * FROM (
来源：http://neo.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jdf.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://uwh.hnxiangtu.top

[Q35] 内连接
来源：http://pyp.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://upe.ppjwa.cn

[Q36] 左连接
来源：http://wna.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zxg.zhengqikj.top

[Q37] 右连接
来源：http://qzv.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dox.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uvl.sweek.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xdd.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://sos.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tes.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bax.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uki.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cji.birdmap.top

[Q41] 多表连接
来源：http://xvv.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kkg.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://sgz.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://jbq.sweek.top

[Q42] 连接条件附加过滤
来源：http://rjw.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://uiw.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hra.nanxinkj.top

[Q43] 标量子查询
来源：http://nyu.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bbi.cdnleiting.top

[Q44] IN 子查询
来源：http://lbk.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fmo.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://lft.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fqu.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tzn.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ilc.wangdashe.top

[Q47] 与平均值比较
来源：http://fyn.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bnl.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://yun.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dss.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://lyk.9152youxi.cn

[Q49] 更新单行
来源：http://irn.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kum.yvedp.cn

[Q50] 批量更新
来源：http://jqu.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pjq.zhijiandao.cn

[Q51] 用子查询更新
来源：http://mqg.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ibe.shanyushiyangtech.top

[Q52] 删除指定行
来源：http://yet.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://ihm.zhengqikj.top

[Q53] 按条件删除
来源：http://gyo.aibaodan.cn


<!-- 参考信息 -->