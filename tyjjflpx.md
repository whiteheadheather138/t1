代发 wailian999

Ruby: s == s.reverse
来源：http://irs.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mbl.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://vyl.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pze.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sqm.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lyp.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://cjd.meibo888.top

Java: // 手写 HashMap
来源：http://vjv.bjfxy.top

Go:   // 手写 map[int]int
来源：http://xpg.ybcxt.top

Ruby: // 手写 Hash
来源：http://mmt.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://hgm.havefunace.top

[N08] 生成全排列
来源：http://ico.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://jjz.yonumen.top

PHP:  // 手写递归交换
来源：http://dju.epnwcf.com

JS:   // 手写回溯递归
来源：http://adl.yj202588.top

TS:   // 手写回溯递归
来源：http://xaq.xuanzx.com

Java: // 手写回溯递归
来源：http://hji.svipenyu.cn

Go:   // 手写回溯递归
来源：http://qit.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://zxl.tianlin.xyz

C#:   // 手写回溯递归
来源：http://gug.cdnleiting.top

[N09] 栈与队列
来源：http://xya.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rwi.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jzg.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rsy.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://syf.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vkc.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bbz.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lch.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bum.pengpengdd.cyou

[N10] 链表节点定义
来源：http://mzi.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bmr.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tok.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fwt.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ooq.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://ock.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://yzk.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://pig.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://hrq.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://spj.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pgd.guowangkeji.top

PHP:  // 手写递归函数
来源：http://efp.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gmi.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eor.yfazqb.com

Java: // 手写递归
来源：http://ewo.hfpthk.cn

Go:   // 手写递归
来源：http://oqd.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gqz.ctjpmb.com

C#:   // 手写递归
来源：http://pfk.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qao.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oof.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ilz.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ixs.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pwm.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ekq.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wsp.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sip.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rop.fengsongda.top

================================================================================
来源：http://nxs.daxiang520.top

O. 并发与异步
来源：http://bus.zhijiandao.cn

================================================================================
来源：http://uuf.52xcode.cn

[O01] 启动一个线程
来源：http://ipe.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yrv.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cxu.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cgh.zhijiandao.cn

TS:   // 同 JS
来源：http://dem.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://ifa.hysaishi.cn

Go:   go f()
来源：http://sbo.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://qui.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://fuk.ydjk.org.cn

[O02] 使用线程池
来源：http://wwl.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gal.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wtb.tarul.cn

JS:   // worker_threads 线程池
来源：http://fpy.yvedp.cn

TS:   // worker_threads 线程池
来源：http://fea.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ubi.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kox.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://njf.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xjp.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://mkf.hfpthk.cn

Py:   with lock: shared += 1
来源：http://rtu.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://rtu.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qtt.meibo888.top

TS:   // 同 JS
来源：http://ljw.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://kec.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qnm.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wsg.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://zez.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://oog.yj202588.top

Py:   async def f():⏎    await g()
来源：http://wwx.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vum.ybcxt.top

JS:   async function f() { await g(); }
来源：http://aar.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ejl.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qih.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://via.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://zqy.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://kmp.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://yvk.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://cdb.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ido.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://weq.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://umg.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dlk.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gwz.xylfe.cn

Ruby: threads.map(&:join)
来源：http://nau.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nfm.fehbvm.com

[O06] 使用进程池
来源：http://mxo.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://djr.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ngi.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://xcr.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://cik.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mis.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://obl.ppjwa.cn

Ruby: // fork 块
来源：http://hrb.shangyingyoupin.top

C#:   Parallel.For
来源：http://hwx.fktsv.cn

================================================================================
来源：http://xtp.daxiang520.top

P. 常用工具函数
来源：http://ulc.nanxuanxn.top

================================================================================
来源：http://pcd.9152youxi.cn

[P01] 生成 UUID
来源：http://psg.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://ymm.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wjl.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://ijh.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://fvl.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://hfa.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://iym.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://sjj.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://lzl.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://wrm.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://joz.daxiang520.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wyg.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hwu.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pdc.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ygp.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ehi.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mjq.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eim.dashuyun.cn

[P03] 生成短随机字符串
来源：http://vvc.gzhubu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oep.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sbk.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lrr.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qvw.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://elb.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pwp.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://tdw.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ckq.svipenyu.cn

[P04] 求长度
来源：http://btl.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fql.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tfe.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bjs.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vmn.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://bdh.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://umd.nanxinkj.top

Ruby: x.length;  x.size
来源：http://pxs.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://itc.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://znf.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://cms.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kwh.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vbc.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bwu.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zix.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ris.zhaomingkeji.xyz

Ruby: a == b
来源：http://qbw.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pxb.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fcb.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qrn.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://kip.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iql.zhengqikj.top

TS:   if (x == null) {}
来源：http://zwh.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hqt.pycfn.com

Go:   if x == nil {}
来源：http://tjr.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ejk.cheryme.top

C#:   if (x is null) {}
来源：http://pcs.smart0.xyz

[P07] 防抖与节流
来源：http://jpn.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rxe.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://suy.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzh.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mih.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gri.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hxi.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://sqx.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zur.cucudq.cn

[P08] 处理浮点精度问题
来源：http://ttf.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wmg.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wkp.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xiv.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://glp.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ihx.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wyy.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vof.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bcq.cdnleiting.top

================================================================================
来源：http://ghs.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aje.mhx1999.top

================================================================================
来源：http://nzg.smart0.xyz

[Q01] 创建表
来源：http://uwo.jqgufenzy.top

CREATE TABLE users (
来源：http://reh.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uri.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://leb.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://swz.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kor.jianghu66.top

);
来源：http://xpr.wangshuangyany.cn

[Q02] 创建带外键的表
来源：http://dkf.snrcjt.cn

CREATE TABLE orders (
来源：http://blr.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iog.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://syv.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://jho.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ocp.shanyushiyangkeji.top

);
来源：http://znp.ctjpmb.com

[Q03] 增加列
来源：http://aqc.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cdt.zdbjq.cn

[Q04] 修改列类型
来源：http://juo.pycfn.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zif.snrcjt.cn

[Q05] 重命名列
来源：http://ili.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aei.aibaodan.cn

[Q06] 删除列
来源：http://fps.meibo888.top

ALTER TABLE users DROP COLUMN age;
来源：http://iyr.xuetiantiany.cn

[Q07] 删除表
来源：http://sqm.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://nrd.havefunace.top

[Q08] 创建普通索引
来源：http://ivm.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xlr.cucudq.cn

[Q09] 创建唯一索引
来源：http://ayh.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hsh.sufxvd.cn

[Q10] 插入单行
来源：http://hqj.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cog.jqgfzy.top

[Q11] 一次插入多行
来源：http://phn.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pus.aizwys.cn

[Q12] 插入后取自增 ID
来源：http://brf.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sdr.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ihd.jinqigufen.top

[Q13] 忽略重复插入
来源：http://qyd.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tdq.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://vdt.tarul.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ivp.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fty.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://ljf.yj20258.top

SELECT * FROM users;
来源：http://cvu.gzhubu.top

[Q16] 查询指定列
来源：http://wsp.tanke756.top

SELECT id, name FROM users;
来源：http://hjl.vqdsnc.cn

[Q17] 条件查询
来源：http://ued.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://huq.smart0.xyz

[Q18] 模糊匹配
来源：http://ddt.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jma.gzhubu.top

[Q19] 范围查询
来源：http://gnr.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tyl.chenlongwang.top

[Q20] IN 列表
来源：http://ibi.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mkf.jinghuilouyu.cn

[Q21] 空值判断
来源：http://tjn.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://njx.hfpthk.cn

[Q22] 排序
来源：http://hlw.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iuk.shzxlz.cn

[Q23] 分页
来源：http://bia.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qwv.yangfankeji.com

[Q24] 去重
来源：http://aqr.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://abz.iojbl.cn

[Q25] 只取前 N 条
来源：http://iik.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://unx.0kj1m.cn

[Q26] 计数
来源：http://byr.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://qzs.dashuyun.cn

[Q27] 条件计数
来源：http://fgk.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aps.xuetiantiany.cn

[Q28] 求和与平均
来源：http://wkd.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ope.yfazqb.com

[Q29] 最大最小值
来源：http://yoo.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://usv.bjfxy.top

[Q30] 分组统计
来源：http://ayq.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vhh.dianchejie.cn

[Q31] 分组后过滤
来源：http://ezw.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yzi.nwbrower.top

[Q32] 分组拼接字符串
来源：http://tod.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://smg.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mgk.sjlbkw.cn

[Q33] 多列分组
来源：http://nma.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hfz.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://tsm.tarul.cn

SELECT * FROM (
来源：http://hsj.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ggw.aizwys.cn

) t WHERE rn = 1;
来源：http://zcu.shanyushiyangtech.top

[Q35] 内连接
来源：http://mjb.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sye.yanxiufei.cn

[Q36] 左连接
来源：http://tpx.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uzb.yj202588.top

[Q37] 右连接
来源：http://mvy.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cty.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://axb.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iev.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://nqf.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hih.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mib.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eed.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dtj.fanxiaobao.xyz

[Q41] 多表连接
来源：http://jti.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://hmt.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://fdo.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://yzx.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://zbz.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://ijp.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://smh.sysykeji.top

[Q43] 标量子查询
来源：http://qck.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zur.epnwcf.com

[Q44] IN 子查询
来源：http://fxi.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zll.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://ycr.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yda.hywenlv.cn


<!-- 参考信息 -->