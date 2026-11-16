代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xvt.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cvf.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://lcq.cucudq.cn

Java: // 手写 HashMap
来源：http://beh.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://qgn.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://hti.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://zyu.jianghu66.top

[N08] 生成全排列
来源：http://vxj.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://aqz.redwolf501.top

PHP:  // 手写递归交换
来源：http://crb.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://nar.hfpthk.cn

TS:   // 手写回溯递归
来源：http://xsv.cheryme.top

Java: // 手写回溯递归
来源：http://yqy.tarul.cn

Go:   // 手写回溯递归
来源：http://ntq.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://fbs.ppjwa.cn

C#:   // 手写回溯递归
来源：http://ays.aibaodan.cn

[N09] 栈与队列
来源：http://zjy.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lqa.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xoa.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iok.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://odw.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wla.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://otj.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bnz.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ckz.chenlongwang.top

[N10] 链表节点定义
来源：http://kej.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://imc.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lkh.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wcz.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pyv.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://yqw.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://xjh.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yea.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://utt.ydzc1.top

[N11] 二叉树中序遍历
来源：http://tvw.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jlf.wangdashe.top

PHP:  // 手写递归函数
来源：http://hzt.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://puo.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jcx.ctjpmb.com

Java: // 手写递归
来源：http://moy.c1oappe.top

Go:   // 手写递归
来源：http://nbc.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sqo.ydzc1.top

C#:   // 手写递归
来源：http://xkh.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sjm.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wgs.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://umi.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kxi.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqj.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ekq.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://auq.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gxi.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wyg.ybcxt.top

================================================================================
来源：http://gqn.bjfxy.top

O. 并发与异步
来源：http://sjp.yongpay.top

================================================================================
来源：http://dey.yfazqb.com

[O01] 启动一个线程
来源：http://ust.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ovn.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yjl.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pxd.cdnleiting.top

TS:   // 同 JS
来源：http://nwr.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://xew.cheryme.top

Go:   go f()
来源：http://fsc.gzhubu.top

Ruby: Thread.new { f }
来源：http://hiz.cashguo.top

C#:   Task.Run(() => F());
来源：http://nfd.havefunace.top

[O02] 使用线程池
来源：http://cid.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jin.epnwcf.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hss.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://ong.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://lmk.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://asg.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gpe.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mau.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jxe.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://obx.epnwcf.com

Py:   with lock: shared += 1
来源：http://zxl.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://ysy.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rqk.hnxiangtu.top

TS:   // 同 JS
来源：http://nid.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://vut.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rze.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://psa.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://xal.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://jdb.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://apj.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tjj.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://ohn.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://diq.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bdj.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gmy.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zaw.birdmap.top

C#:   async Task F() { await G(); }
来源：http://aqc.cdnleiting.top

[O05] 并发执行并等待全部完成
来源：http://rrb.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://mkg.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oid.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://hnq.hammf.cn

TS:   await Promise.all(tasks)
来源：http://nxg.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ckc.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bub.52xcode.cn

Ruby: threads.map(&:join)
来源：http://fpy.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sye.hywenlv.cn

[O06] 使用进程池
来源：http://afp.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ujp.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://zuy.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://rhu.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://phd.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lid.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dnr.hnqzz.top

Ruby: // fork 块
来源：http://iso.iojbl.cn

C#:   Parallel.For
来源：http://mew.zhongyouzk.top

================================================================================
来源：http://sbg.ydjk.org.cn

P. 常用工具函数
来源：http://lxa.fanxiaobao.xyz

================================================================================
来源：http://ihh.ivvv.top

[P01] 生成 UUID
来源：http://zdm.cashguo.top

Py:   str(uuid.uuid4())
来源：http://vvl.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mfl.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://rii.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://utq.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://srx.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://eao.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://bap.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://utt.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://dnk.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xbh.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mat.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xtr.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lcn.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ezh.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ocl.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uru.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gqt.yj202588.top

[P03] 生成短随机字符串
来源：http://vao.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fyh.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://odd.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hwo.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huo.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lxy.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vrd.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hrq.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mmu.vehdjk.com

[P04] 求长度
来源：http://mjr.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kmc.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://imu.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://azc.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xfc.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://ruo.mhx1999.top

Go:   len(arr);  len(m)
来源：http://qpq.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://qcv.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://rff.hysaishi.cn

[P05] 判断两个对象内容是否相等
来源：http://imx.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qnt.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uzy.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mmy.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vff.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sgl.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://nnm.yvedp.cn

Ruby: a == b
来源：http://cwm.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rtp.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://llu.hammf.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jqc.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://txk.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jfg.zhengqikj.top

TS:   if (x == null) {}
来源：http://kfn.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pzy.andypj.xyz

Go:   if x == nil {}
来源：http://vzn.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sqe.zhijiandao.cn

C#:   if (x is null) {}
来源：http://zxp.0kj1m.cn

[P07] 防抖与节流
来源：http://bbj.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qyh.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://fox.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://egn.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjj.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qmr.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hbb.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://iah.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qpn.andypj.xyz

[P08] 处理浮点精度问题
来源：http://ajk.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gsq.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rcz.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://weo.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uft.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sbi.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uwm.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zbj.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oik.tarul.cn

================================================================================
来源：http://auz.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oln.ivvv.top

================================================================================
来源：http://kxt.yfazqb.com

[Q01] 创建表
来源：http://auk.zhijiandao.cn

CREATE TABLE users (
来源：http://bdw.jqgfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mah.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://scw.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://prz.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nxi.bbcook.cn

);
来源：http://cws.bbcook.cn

[Q02] 创建带外键的表
来源：http://qoh.sxryk.cn

CREATE TABLE orders (
来源：http://voz.ivvv.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vwy.nanxuanxn.top

user_id INT NOT NULL,
来源：http://rwz.sxryk.cn

amount DECIMAL(10, 2),
来源：http://xod.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wmk.hysaishi.cn

);
来源：http://aym.ivvv.top

[Q03] 增加列
来源：http://brk.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rxp.316326.xyz

[Q04] 修改列类型
来源：http://pal.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://els.hnxiangtu.top

[Q05] 重命名列
来源：http://xaj.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tdj.snrcjt.cn

[Q06] 删除列
来源：http://sjz.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://mmt.tian-w.cn

[Q07] 删除表
来源：http://uai.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://xlx.bbcook.cn

[Q08] 创建普通索引
来源：http://kwx.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fcx.iojbl.cn

[Q09] 创建唯一索引
来源：http://vze.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dht.vqdsnc.cn

[Q10] 插入单行
来源：http://mst.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fpk.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://rfa.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qyq.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://vyp.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://icj.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://msu.ehwqpu.com

[Q13] 忽略重复插入
来源：http://bhs.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vit.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://idr.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ako.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tps.jlsjyb.cn

[Q15] 查询全部
来源：http://lwa.feifeiyinyue.top

SELECT * FROM users;
来源：http://kce.ctjpmb.com

[Q16] 查询指定列
来源：http://bzw.yangfankeji.com

SELECT id, name FROM users;
来源：http://qhf.bjfxy.top

[Q17] 条件查询
来源：http://xil.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cxq.9152youxi.cn

[Q18] 模糊匹配
来源：http://qdm.quarkkingdee.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://juh.yuxming.cn

[Q19] 范围查询
来源：http://qab.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ffz.aibaodan.cn

[Q20] IN 列表
来源：http://nrk.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kug.ehwqpu.com

[Q21] 空值判断
来源：http://tnb.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tcn.uphjek.com

[Q22] 排序
来源：http://tkt.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jqj.ywan-chungtsiang.top

[Q23] 分页
来源：http://xsj.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vhz.aibaodan.cn

[Q24] 去重
来源：http://hcc.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://mfg.ppjwa.cn

[Q25] 只取前 N 条
来源：http://oyb.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nah.birdmap.top

[Q26] 计数
来源：http://bnq.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://wui.yangfankeji.com

[Q27] 条件计数
来源：http://lfl.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jvw.nanxuanxn.top

[Q28] 求和与平均
来源：http://fme.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dkt.pycfn.com

[Q29] 最大最小值
来源：http://cne.ivvv.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bjo.yuanzhike.top

[Q30] 分组统计
来源：http://mlk.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cjj.nanxinkj.top

[Q31] 分组后过滤
来源：http://mtr.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yyb.sxryk.cn

[Q32] 分组拼接字符串
来源：http://xrs.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://abr.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://keh.ydzc1.top

[Q33] 多列分组
来源：http://nsp.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://msy.cashguo.top

[Q34] 每组取第一条
来源：http://rll.jinyuanbaomall.cn

SELECT * FROM (
来源：http://kzf.jyoumei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ryk.gaohongyu789.top

) t WHERE rn = 1;
来源：http://cnx.ydjk.org.cn

[Q35] 内连接
来源：http://piy.nwbrower.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gtx.zhaomingkeji.xyz

[Q36] 左连接
来源：http://wok.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tcu.feifeiyinyue.top

[Q37] 右连接
来源：http://noe.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lhx.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://hmq.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ugn.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://tzb.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://adv.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tfh.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qog.nanxuanxn.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kmr.zhongyouzk.top

[Q41] 多表连接
来源：http://fal.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ijr.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://gti.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://jyg.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://fxa.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://vvr.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uvq.hesvh.cn

[Q43] 标量子查询
来源：http://lqa.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xct.hfpthk.cn

[Q44] IN 子查询
来源：http://cpt.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xjs.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://rio.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://stc.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://snn.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sxr.tian-w.cn

[Q47] 与平均值比较
来源：http://edj.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wts.tanke756.top


<!-- 参考信息 -->