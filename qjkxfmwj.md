代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fxq.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xiw.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://ngh.jianghu66.top

Java: // 手写 HashMap
来源：http://xbx.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://utx.dianchejie.cn

Ruby: // 手写 Hash
来源：http://lbk.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cjx.sjlbkw.cn

[N08] 生成全排列
来源：http://vqm.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://lvp.tanke756.top

PHP:  // 手写递归交换
来源：http://tts.cdnleiting.top

JS:   // 手写回溯递归
来源：http://xfw.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://fle.yfazqb.com

Java: // 手写回溯递归
来源：http://dcr.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://kag.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://pqz.gotoacloud.top

C#:   // 手写回溯递归
来源：http://fza.tianlin.xyz

[N09] 栈与队列
来源：http://rsp.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ttv.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cmv.jianghu66.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kly.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yko.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kuo.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gnj.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://orc.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fpo.gogol.net.cn

[N10] 链表节点定义
来源：http://fwv.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qij.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cvv.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gxd.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ioz.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://ydn.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cwm.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://guf.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cuv.aizwys.cn

[N11] 二叉树中序遍历
来源：http://bfa.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gpn.sysykeji.top

PHP:  // 手写递归函数
来源：http://adi.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tng.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bim.jiagoushi.top

Java: // 手写递归
来源：http://fmq.hfpthk.cn

Go:   // 手写递归
来源：http://iup.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kdo.hysaishi.cn

C#:   // 手写递归
来源：http://oxk.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ucg.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wlg.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pzy.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nfs.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gms.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pif.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qup.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hig.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fiz.pycfn.com

================================================================================
来源：http://fqn.tanke756.top

O. 并发与异步
来源：http://oxd.shuidangran.top

================================================================================
来源：http://tpv.zhiwuduotai.top

[O01] 启动一个线程
来源：http://grq.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vwo.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nsm.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wcv.daxiang520.top

TS:   // 同 JS
来源：http://eaa.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://ikf.fengsongda.top

Go:   go f()
来源：http://tvu.nanxinkj.top

Ruby: Thread.new { f }
来源：http://jvb.wangdashe.top

C#:   Task.Run(() => F());
来源：http://sfg.ctjpmb.com

[O02] 使用线程池
来源：http://gsn.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://idg.fzhhl.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nzw.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://wia.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://ixu.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://cae.cdnleiting.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dmc.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qpz.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://krh.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://nub.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://wtv.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://raa.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pjg.zhixingplan.top

TS:   // 同 JS
来源：http://yur.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://hcd.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://syo.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wxg.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://uwm.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://pvs.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://irr.c1oappe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dhg.epnwcf.com

JS:   async function f() { await g(); }
来源：http://udz.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ngd.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rlj.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pjf.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://pyy.yonumen.top

C#:   async Task F() { await G(); }
来源：http://qza.hywenlv.cn

[O05] 并发执行并等待全部完成
来源：http://uka.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://iuz.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://evb.uphjek.com

JS:   await Promise.all(tasks)
来源：http://mwm.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://mcd.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zkg.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gdi.9152youxi.cn

Ruby: threads.map(&:join)
来源：http://cqk.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nqs.cashguo.top

[O06] 使用进程池
来源：http://oev.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wzd.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tvv.fehbvm.com

JS:   // child_process / cluster 模块
来源：http://qni.meibo888.top

TS:   // child_process / cluster 模块
来源：http://hlh.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dqx.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dqb.fzhhl.top

Ruby: // fork 块
来源：http://lsh.daxiang520.top

C#:   Parallel.For
来源：http://jqm.tian-w.cn

================================================================================
来源：http://ndr.wangshuangyany.cn

P. 常用工具函数
来源：http://eaq.tarul.cn

================================================================================
来源：http://ehr.andypj.xyz

[P01] 生成 UUID
来源：http://nmg.ivvv.top

Py:   str(uuid.uuid4())
来源：http://lfn.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://khk.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://qge.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://lxe.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://duu.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://szt.pycfn.com

Ruby: SecureRandom.uuid
来源：http://hiy.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://ygn.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://tww.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vmh.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://awy.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://quy.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mta.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dqk.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://frm.fktsv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ryz.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lsq.zycfv.cn

[P03] 生成短随机字符串
来源：http://zol.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pbw.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jfj.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://juw.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aru.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oxp.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jsl.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://eog.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bts.hesvh.cn

[P04] 求长度
来源：http://jjt.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wrm.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uhx.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qmt.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://onf.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://mlt.daxiang520.top

Go:   len(arr);  len(m)
来源：http://uei.gotoacloud.top

Ruby: x.length;  x.size
来源：http://erm.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wcg.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://ibc.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mya.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vsz.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rng.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://omy.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bec.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://rus.zdbjq.cn

Ruby: a == b
来源：http://btg.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://abq.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lth.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tnb.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://uao.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cyi.fzhhl.top

TS:   if (x == null) {}
来源：http://hys.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gcg.tarul.cn

Go:   if x == nil {}
来源：http://iyr.hammf.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ytk.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://ghm.dashuyun.cn

[P07] 防抖与节流
来源：http://elx.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cds.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://fke.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tdf.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mss.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mmz.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hrg.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fei.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ljx.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://stp.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yzl.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sbn.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kod.xuanzx.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uqa.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wvx.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gzq.tianlin.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://znc.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jnv.gaohongyu789.top

================================================================================
来源：http://hfg.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vpr.shzxlz.cn

================================================================================
来源：http://vdu.fanxiaobao.xyz

[Q01] 创建表
来源：http://bds.hnxiangtu.top

CREATE TABLE users (
来源：http://ybj.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://otk.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://smn.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://vhw.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jib.jqgufenzy.top

);
来源：http://oqu.0kj1m.cn

[Q02] 创建带外键的表
来源：http://rzj.yanxiufei.cn

CREATE TABLE orders (
来源：http://syg.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fuq.fehbvm.com

user_id INT NOT NULL,
来源：http://jtn.bbcook.cn

amount DECIMAL(10, 2),
来源：http://inc.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lzl.meibo888.top

);
来源：http://ego.bjfxy.top

[Q03] 增加列
来源：http://fhb.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pkx.hcnkem.com

[Q04] 修改列类型
来源：http://gth.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rnr.9152youxi.cn

[Q05] 重命名列
来源：http://ifv.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mzk.zhiwuduotai.top

[Q06] 删除列
来源：http://oxq.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://zix.jinghuilouyu.cn

[Q07] 删除表
来源：http://dbv.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://fve.tanke756.top

[Q08] 创建普通索引
来源：http://hkp.pycfn.com

CREATE INDEX idx_users_email ON users(email);
来源：http://aml.52xcode.cn

[Q09] 创建唯一索引
来源：http://fbt.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kzw.shuidangran.top

[Q10] 插入单行
来源：http://cfq.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hjb.xuanzx.com

[Q11] 一次插入多行
来源：http://nwg.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tub.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://xhw.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://zaa.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nep.shzxlz.cn

[Q13] 忽略重复插入
来源：http://yvt.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ayf.wangdashe.top

[Q14] 存在则更新（upsert）
来源：http://jej.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lbo.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cit.birdmap.top

[Q15] 查询全部
来源：http://rlj.cheryme.top

SELECT * FROM users;
来源：http://fai.aibaodan.cn

[Q16] 查询指定列
来源：http://tce.sysykeji.top

SELECT id, name FROM users;
来源：http://uqd.feifeiyinyue.top

[Q17] 条件查询
来源：http://uag.aibaodan.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eiw.jqgufenzy.top

[Q18] 模糊匹配
来源：http://qtm.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jig.wangdashe.top

[Q19] 范围查询
来源：http://cfg.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cvg.ppjwa.cn

[Q20] IN 列表
来源：http://sgs.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://inc.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://hzc.fktsv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hdx.meibo888.top

[Q22] 排序
来源：http://ble.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yac.shanyushiyangtech.top

[Q23] 分页
来源：http://qup.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hzf.c1oappe.top

[Q24] 去重
来源：http://ewr.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://htp.sweek.top

[Q25] 只取前 N 条
来源：http://doi.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://prc.epnwcf.com

[Q26] 计数
来源：http://nds.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://pkw.havefunace.top

[Q27] 条件计数
来源：http://hkj.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://est.chenzaomai.com

[Q28] 求和与平均
来源：http://bvz.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cuh.9152youxi.cn

[Q29] 最大最小值
来源：http://uho.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qbb.jqgfzy.top

[Q30] 分组统计
来源：http://ofr.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jyg.sysykeji.top

[Q31] 分组后过滤
来源：http://xwk.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jot.smart0.xyz

[Q32] 分组拼接字符串
来源：http://slv.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mzk.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bva.yonumen.top

[Q33] 多列分组
来源：http://eaf.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pni.iojbl.cn

[Q34] 每组取第一条
来源：http://kpt.fanxiaobao.xyz

SELECT * FROM (
来源：http://got.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nck.meibo888.top

) t WHERE rn = 1;
来源：http://pdt.hongshengwenyu.top

[Q35] 内连接
来源：http://bzb.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mbk.fanxiaobao.xyz

[Q36] 左连接
来源：http://akh.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hhg.zhongyouzk.top

[Q37] 右连接
来源：http://xtz.meibo888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vzu.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://ecs.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://maf.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://qbg.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://awu.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xvd.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dpk.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vbf.jianghu66.top

[Q41] 多表连接
来源：http://bqa.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lqh.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://zps.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://ock.vehdjk.com

[Q42] 连接条件附加过滤
来源：http://hrh.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://epo.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xfj.aizwys.cn

[Q43] 标量子查询
来源：http://oig.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lpn.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://hld.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ime.birdmap.top

[Q45] EXISTS 判断存在
来源：http://nys.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mwy.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://ime.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yih.dianchejie.cn

[Q47] 与平均值比较
来源：http://czg.cheryme.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pii.sjlbkw.cn


<!-- 参考信息 -->