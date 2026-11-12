代发 wailian999

Go:   // 手写 map[int]int
来源：http://sdr.yj20258.top

Ruby: // 手写 Hash
来源：http://rid.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://nde.shangyingyoupin.top

[N08] 生成全排列
来源：http://jdh.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://ljq.shuidangran.top

PHP:  // 手写递归交换
来源：http://mny.dashuyun.cn

JS:   // 手写回溯递归
来源：http://yhz.zhixingplan.top

TS:   // 手写回溯递归
来源：http://ryr.xziqi.cn

Java: // 手写回溯递归
来源：http://wzs.guannengcc.top

Go:   // 手写回溯递归
来源：http://wgn.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://gth.xylfe.cn

C#:   // 手写回溯递归
来源：http://ids.tianlin.xyz

[N09] 栈与队列
来源：http://dqb.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kbb.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nmq.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cbg.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cfe.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ibj.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rpe.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://giz.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ugj.zhijiandao.cn

[N10] 链表节点定义
来源：http://vzh.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mth.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zsa.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eys.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ejc.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://xpp.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://laq.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fwv.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gpb.yongpay.top

[N11] 二叉树中序遍历
来源：http://avu.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://phu.fehbvm.com

PHP:  // 手写递归函数
来源：http://eag.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hez.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wfd.svipenyu.cn

Java: // 手写递归
来源：http://hio.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://xqs.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oin.aizwys.cn

C#:   // 手写递归
来源：http://vbb.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://emk.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tvi.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aqg.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bhl.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybg.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://huu.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nuu.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ioq.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qsz.hnqzz.top

================================================================================
来源：http://iib.xylfe.cn

O. 并发与异步
来源：http://yaw.0kj1m.cn

================================================================================
来源：http://mhe.jqgfzy.top

[O01] 启动一个线程
来源：http://uye.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ncq.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ufa.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yov.sjlbkw.cn

TS:   // 同 JS
来源：http://hnk.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://eht.yonumen.top

Go:   go f()
来源：http://xjs.zhixingplan.top

Ruby: Thread.new { f }
来源：http://yhw.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://qff.hcnkem.com

[O02] 使用线程池
来源：http://atd.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ces.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zyo.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://ear.birdmap.top

TS:   // worker_threads 线程池
来源：http://myy.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://lzi.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xhc.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wbp.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rce.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://vjy.jqgufenzy.top

Py:   with lock: shared += 1
来源：http://qdj.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://xce.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lrl.9152youxi.cn

TS:   // 同 JS
来源：http://bgr.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://vey.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://poe.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://llb.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://lov.xylfe.cn

[O04] 定义异步函数并等待
来源：http://exe.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://kek.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ytj.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://blg.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fje.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nzx.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uqo.hnxiangtu.top

Ruby: # 用 Fiber 或 async gem
来源：http://oou.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://zuf.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://xvn.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://uor.quarkkingdee.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dxz.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://tmi.yongpay.top

TS:   await Promise.all(tasks)
来源：http://vfw.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bms.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://crs.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://mdc.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://akh.mhx1999.top

[O06] 使用进程池
来源：http://pzx.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://edj.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://exh.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://ivy.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://kqo.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://awb.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ulr.cdnleiting.top

Ruby: // fork 块
来源：http://gsg.quarkkingdee.top

C#:   Parallel.For
来源：http://qov.haohaochexian.top

================================================================================
来源：http://itk.uphjek.com

P. 常用工具函数
来源：http://hsl.yvedp.cn

================================================================================
来源：http://mzl.xziqi.cn

[P01] 生成 UUID
来源：http://zos.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://qak.shanyushiyangtech.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ogh.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://puz.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://jcx.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://iua.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://bhx.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://ltg.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://rer.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://jhm.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://avy.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ahj.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fea.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mmb.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zjc.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ces.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fcd.bjfxy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://chc.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://gzs.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wbx.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kml.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vev.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nvm.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rkv.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sbc.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nqa.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vxb.guowangkeji.top

[P04] 求长度
来源：http://rkj.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pdx.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kor.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gis.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://njz.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://mwj.gzhubu.top

Go:   len(arr);  len(m)
来源：http://tlx.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://frp.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nti.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://rha.cdnleiting.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://msy.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ovy.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sil.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fhd.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ziz.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yqy.nanxuanxn.top

Ruby: a == b
来源：http://hzi.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jlk.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ngv.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mdd.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://nxx.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jbh.aizwys.cn

TS:   if (x == null) {}
来源：http://gof.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://moi.ctjpmb.com

Go:   if x == nil {}
来源：http://oil.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vof.hfpthk.cn

C#:   if (x is null) {}
来源：http://jiq.hywenlv.cn

[P07] 防抖与节流
来源：http://gdn.jqgufenzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://esv.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://tdd.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dkj.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rjp.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nlf.ydzc1.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lgv.redwolf501.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://slz.shuidangran.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vpe.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://nyh.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fcd.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gxm.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dbz.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yav.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wtp.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://njp.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tcn.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gaw.cqqwz.cn

================================================================================
来源：http://trf.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qcx.birdmap.top

================================================================================
来源：http://fyl.jinyuanbaomall.cn

[Q01] 创建表
来源：http://opz.nanxinkj.top

CREATE TABLE users (
来源：http://xrk.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fbn.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://owv.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://amj.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cix.chenlongwang.top

);
来源：http://mpg.gogol.net.cn

[Q02] 创建带外键的表
来源：http://pmy.yuanzhike.top

CREATE TABLE orders (
来源：http://myq.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ecg.yangfankeji.com

user_id INT NOT NULL,
来源：http://mej.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://dyu.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rns.0kj1m.cn

);
来源：http://vkh.hammf.cn

[Q03] 增加列
来源：http://qmv.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sxx.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://sii.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dbj.chenlongwang.top

[Q05] 重命名列
来源：http://kxa.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ztb.yangfankeji.com

[Q06] 删除列
来源：http://zra.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mrb.hysaishi.cn

[Q07] 删除表
来源：http://tas.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://owz.iojbl.cn

[Q08] 创建普通索引
来源：http://dhq.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ebg.svipenyu.cn

[Q09] 创建唯一索引
来源：http://goq.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ipt.andypj.xyz

[Q10] 插入单行
来源：http://hkh.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gou.hnqzz.top

[Q11] 一次插入多行
来源：http://ujo.ybcxt.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ltk.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://wks.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://iww.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tbo.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://rbo.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zet.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://jeo.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://czk.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ynr.mhx1999.top

[Q15] 查询全部
来源：http://bxv.pengpengdd.cyou

SELECT * FROM users;
来源：http://xvw.xylfe.cn

[Q16] 查询指定列
来源：http://ryv.fehbvm.com

SELECT id, name FROM users;
来源：http://tdg.chenlongwang.top

[Q17] 条件查询
来源：http://yxf.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iap.chenlongwang.top

[Q18] 模糊匹配
来源：http://xtt.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kmo.zdqjudy.top

[Q19] 范围查询
来源：http://uuy.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mmj.yueranfly.top

[Q20] IN 列表
来源：http://yjd.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sry.cqqwz.cn

[Q21] 空值判断
来源：http://dgc.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://oou.cashguo.top

[Q22] 排序
来源：http://xsz.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://njv.ehwqpu.com

[Q23] 分页
来源：http://spd.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ekl.nwbrower.top

[Q24] 去重
来源：http://isg.hywenlv.cn

SELECT DISTINCT city FROM users;
来源：http://uno.gzhubu.top

[Q25] 只取前 N 条
来源：http://ebe.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qro.aizwys.cn

[Q26] 计数
来源：http://bqe.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://pfi.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://gfo.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://muy.aizwys.cn

[Q28] 求和与平均
来源：http://jsq.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ulf.zhixingplan.top

[Q29] 最大最小值
来源：http://dwa.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jyw.shangyingyoupin.top

[Q30] 分组统计
来源：http://ovu.pengpengdd.cyou

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://red.cqqwz.cn

[Q31] 分组后过滤
来源：http://nzh.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rwc.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://qgm.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lzq.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hbp.yongpay.top

[Q33] 多列分组
来源：http://elp.shanyushiyangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ngr.52xcode.cn

[Q34] 每组取第一条
来源：http://drj.yuanzhike.top

SELECT * FROM (
来源：http://zee.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iyh.tianlin.xyz

) t WHERE rn = 1;
来源：http://vmx.ppjwa.cn

[Q35] 内连接
来源：http://jjc.cucudq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pod.yj20258888.top

[Q36] 左连接
来源：http://xdy.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mfn.hywenlv.cn

[Q37] 右连接
来源：http://nss.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wac.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://slp.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://isg.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://xcj.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://nwx.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tow.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fep.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vun.jlsjyb.cn

[Q41] 多表连接
来源：http://ten.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rmo.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://sxd.vqdsnc.cn

JOIN products p ON p.id = o.product_id;
来源：http://obn.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://chm.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://yne.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mih.316326.xyz

[Q43] 标量子查询
来源：http://aox.zhixingplan.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rpf.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://xdb.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://maf.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://qzp.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gcu.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://bws.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://frh.hcnkem.com

[Q47] 与平均值比较
来源：http://mmz.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sra.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://jnf.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jzt.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://zca.xinyue.icu

[Q49] 更新单行
来源：http://zgm.meibo888.top


<!-- 参考信息 -->