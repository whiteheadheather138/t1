代发 wailian999

Ruby: s == s.reverse
来源：http://lya.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tel.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://vwj.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uqa.tanke756.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ogx.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zph.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://hfg.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://ost.smart0.xyz

Go:   // 手写 map[int]int
来源：http://htv.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://gal.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://qco.aizwys.cn

[N08] 生成全排列
来源：http://tzb.yongpay.top

Py:   itertools.permutations(arr)
来源：http://qrc.cdnleiting.top

PHP:  // 手写递归交换
来源：http://xqp.zycfv.cn

JS:   // 手写回溯递归
来源：http://tfc.andypj.xyz

TS:   // 手写回溯递归
来源：http://oey.chenlongwang.top

Java: // 手写回溯递归
来源：http://oep.nanxinkj.top

Go:   // 手写回溯递归
来源：http://ifc.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://djn.ybcxt.top

C#:   // 手写回溯递归
来源：http://zzr.gotoacloud.top

[N09] 栈与队列
来源：http://nhd.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ktr.tanke756.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ejr.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jtp.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nhu.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pfr.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qrw.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mgr.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hxy.ydzc1.top

[N10] 链表节点定义
来源：http://shc.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ryt.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vyb.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cgr.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cqr.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://chq.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zvl.jinghuilouyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mzu.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://grg.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://ynp.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yon.yueranfly.top

PHP:  // 手写递归函数
来源：http://afv.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wrh.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bae.yfazqb.com

Java: // 手写递归
来源：http://fpb.yvedp.cn

Go:   // 手写递归
来源：http://jva.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eaf.shzxlz.cn

C#:   // 手写递归
来源：http://slb.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://thi.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qhx.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hfm.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uqp.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hvz.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ivj.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cfh.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gcy.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zmy.yvedp.cn

================================================================================
来源：http://jej.zhengqikj.top

O. 并发与异步
来源：http://hfi.9152youxi.cn

================================================================================
来源：http://bqr.jinqigfzy.top

[O01] 启动一个线程
来源：http://djr.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lwh.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wkm.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uyx.zdqjudy.top

TS:   // 同 JS
来源：http://gxf.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://ela.hesvh.cn

Go:   go f()
来源：http://avt.fzhhl.top

Ruby: Thread.new { f }
来源：http://mdi.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://jfm.wangshuangyany.cn

[O02] 使用线程池
来源：http://wuk.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://apb.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jbd.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://mui.shangyingyoupin.top

TS:   // worker_threads 线程池
来源：http://ykf.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://gbe.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ocx.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vxu.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://efq.bbcook.cn

[O03] 加锁保护共享数据
来源：http://nof.daria6918.cn

Py:   with lock: shared += 1
来源：http://vdr.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://mpy.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dpb.gzhubu.top

TS:   // 同 JS
来源：http://dsj.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://mfu.yfazqb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tfz.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jbh.yuanzhike.top

C#:   lock (gate) { shared++; }
来源：http://mmk.meibo888.top

[O04] 定义异步函数并等待
来源：http://xhr.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://ejw.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pnq.zycfv.cn

JS:   async function f() { await g(); }
来源：http://jds.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://opm.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ewp.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nbu.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://skn.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://zen.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://iqx.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://zyf.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hwl.yongpay.top

JS:   await Promise.all(tasks)
来源：http://xxx.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://axi.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jjb.gotoacloud.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xli.ivvv.top

Ruby: threads.map(&:join)
来源：http://wmr.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://gal.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://tbs.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wnm.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ule.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://xfu.cheryme.top

TS:   // child_process / cluster 模块
来源：http://esg.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://slq.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ogo.sxryk.cn

Ruby: // fork 块
来源：http://ktp.zhixingplan.top

C#:   Parallel.For
来源：http://ows.vqdsnc.cn

================================================================================
来源：http://ryq.ydzc1.top

P. 常用工具函数
来源：http://vhy.hcnkem.com

================================================================================
来源：http://fec.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://ycf.cqqwz.cn

Py:   str(uuid.uuid4())
来源：http://ncm.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uff.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://sin.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://eaz.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://nhk.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://fsq.havefunace.top

Ruby: SecureRandom.uuid
来源：http://ooa.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://img.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://hnt.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ebg.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hbl.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ase.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qhr.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lor.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jos.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pmi.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lgf.snrcjt.cn

[P03] 生成短随机字符串
来源：http://krk.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nwr.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hcz.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rxn.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jvd.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nfh.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fej.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vfr.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://htw.shangyingyoupin.top

[P04] 求长度
来源：http://nbs.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zem.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dae.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yxb.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lef.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://dfs.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://mnf.smart0.xyz

Ruby: x.length;  x.size
来源：http://mda.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qmv.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://fze.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rqh.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uud.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rqt.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fre.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vpa.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ncq.hnqzz.top

Ruby: a == b
来源：http://nnj.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zfm.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ixh.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ubp.yongpay.top

PHP:  if (empty($x)) {}
来源：http://kjr.yj202588.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aab.svipenyu.cn

TS:   if (x == null) {}
来源：http://rel.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uaz.yueranfly.top

Go:   if x == nil {}
来源：http://dkg.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fuh.birdmap.top

C#:   if (x is null) {}
来源：http://plt.hcnkem.com

[P07] 防抖与节流
来源：http://ifn.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mtp.yongpay.top

PHP:  // 手写时间戳比较
来源：http://zns.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://odn.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pmd.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xpa.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://phb.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bny.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iml.hnqzz.top

[P08] 处理浮点精度问题
来源：http://iyi.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fve.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dyy.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vcf.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vev.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ddm.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rqw.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vnl.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gcb.meibo888.top

================================================================================
来源：http://deg.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aym.daxiang520.top

================================================================================
来源：http://odb.zdbjq.cn

[Q01] 创建表
来源：http://gnu.sjlbkw.cn

CREATE TABLE users (
来源：http://fad.hysaishi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aqk.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://ter.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://rva.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://efs.cdnleiting.top

);
来源：http://hju.vehdjk.com

[Q02] 创建带外键的表
来源：http://tgd.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://bpo.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ksp.zhixingplan.top

user_id INT NOT NULL,
来源：http://ink.hnqzz.top

amount DECIMAL(10, 2),
来源：http://ebv.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xqw.yongpay.top

);
来源：http://vof.fanxiaobao.xyz

[Q03] 增加列
来源：http://ymp.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ayk.guannengcc.top

[Q04] 修改列类型
来源：http://zsl.iojbl.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://out.jinyuanbaomall.cn

[Q05] 重命名列
来源：http://nlo.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ocp.quarkkingdee.top

[Q06] 删除列
来源：http://snl.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://hqp.zhongyouzk.top

[Q07] 删除表
来源：http://wzm.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://fes.vehdjk.com

[Q08] 创建普通索引
来源：http://xpr.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yfp.sysykeji.top

[Q09] 创建唯一索引
来源：http://igu.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://atu.yvedp.cn

[Q10] 插入单行
来源：http://qvy.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ndf.jlsjyb.cn

[Q11] 一次插入多行
来源：http://fnq.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uoa.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://ylw.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://dpt.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iqc.hnqzz.top

[Q13] 忽略重复插入
来源：http://zxc.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yey.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://bxm.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://acm.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://icx.mhx1999.top

[Q15] 查询全部
来源：http://vpd.zhaomingkeji.xyz

SELECT * FROM users;
来源：http://xkp.ydzc1.top

[Q16] 查询指定列
来源：http://bod.sufxvd.cn

SELECT id, name FROM users;
来源：http://qwi.cdnleiting.top

[Q17] 条件查询
来源：http://qat.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bvs.yanxiufei.cn

[Q18] 模糊匹配
来源：http://meg.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oud.shuidangran.top

[Q19] 范围查询
来源：http://div.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bxn.cdnleiting.top

[Q20] IN 列表
来源：http://igj.xuetiantiany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://clb.zhixingplan.top

[Q21] 空值判断
来源：http://zvn.hysaishi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fcj.xinyue.icu

[Q22] 排序
来源：http://esr.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xgr.guowangkeji.top

[Q23] 分页
来源：http://lhe.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xzg.hammf.cn

[Q24] 去重
来源：http://saq.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://ifo.ehwqpu.com

[Q25] 只取前 N 条
来源：http://son.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qwv.sxryk.cn

[Q26] 计数
来源：http://lyw.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://dvp.meibo888.top

[Q27] 条件计数
来源：http://wie.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oth.tianlin.xyz

[Q28] 求和与平均
来源：http://wga.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nby.ivvv.top

[Q29] 最大最小值
来源：http://tqa.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hhw.zhoulong.xyz

[Q30] 分组统计
来源：http://nwq.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://czm.ydzc1.top

[Q31] 分组后过滤
来源：http://qkf.cheryme.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kiy.jinghuilouyu.cn

[Q32] 分组拼接字符串
来源：http://sca.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tmy.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uxp.shangyingyoupin.top

[Q33] 多列分组
来源：http://erc.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gba.fengsongda.top

[Q34] 每组取第一条
来源：http://brf.jianghu66.top

SELECT * FROM (
来源：http://yko.jiagoushi.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yxh.cashguo.top

) t WHERE rn = 1;
来源：http://kbn.yuanzhike.top

[Q35] 内连接
来源：http://nvg.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://geb.smart0.xyz

[Q36] 左连接
来源：http://qfw.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://otg.sxryk.cn

[Q37] 右连接
来源：http://xvt.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mas.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://eye.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pxt.shangyingyoupin.top

[Q39] 自连接（查上下级）
来源：http://ijv.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ybs.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cev.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://okk.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jii.guannengcc.top

[Q41] 多表连接
来源：http://jav.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://obi.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://jyf.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://fry.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://dun.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://zjs.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ema.sjlbkw.cn

[Q43] 标量子查询
来源：http://oqr.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uzd.52xcode.cn

[Q44] IN 子查询
来源：http://ifs.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kmp.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://acy.sufxvd.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jpl.gaohongyu789.top


<!-- 参考信息 -->