代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://fyi.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://tmx.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dph.jianghu66.top

Go:   // 双指针从两端比较
来源：http://jzs.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://axk.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zpp.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://yog.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qak.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rbq.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://udi.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://fnf.hnxiangtu.top

Java: // 手写 HashMap
来源：http://qgw.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://xkx.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://isi.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://lsi.fanxiaobao.xyz

[N08] 生成全排列
来源：http://njn.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://qgg.snrcjt.cn

PHP:  // 手写递归交换
来源：http://hoi.zhaomingkeji.xyz

JS:   // 手写回溯递归
来源：http://xyv.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://bcl.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://zsc.yfazqb.com

Go:   // 手写回溯递归
来源：http://hzd.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://oqt.tanke756.top

C#:   // 手写回溯递归
来源：http://jsy.birdmap.top

[N09] 栈与队列
来源：http://rmc.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mwm.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ttf.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wbi.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://isq.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ulk.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xrn.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zzb.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oys.fktsv.cn

[N10] 链表节点定义
来源：http://qju.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://odt.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fzy.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jom.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://noi.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://muk.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://dyl.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://kvf.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tlw.fktsv.cn

[N11] 二叉树中序遍历
来源：http://hgx.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mlr.ybcxt.top

PHP:  // 手写递归函数
来源：http://nlx.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://crt.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cix.shanyushiyangkeji.top

Java: // 手写递归
来源：http://dmq.hfpthk.cn

Go:   // 手写递归
来源：http://nar.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mmr.daxiang520.top

C#:   // 手写递归
来源：http://dsk.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gsv.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qku.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://los.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kba.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nuo.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://met.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ens.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uui.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://trp.dianchejie.cn

================================================================================
来源：http://tao.zdbjq.cn

O. 并发与异步
来源：http://gtn.daria6918.cn

================================================================================
来源：http://yxl.zhoulong.xyz

[O01] 启动一个线程
来源：http://zta.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sny.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://abl.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uac.epnwcf.com

TS:   // 同 JS
来源：http://zht.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://bkn.mhx1999.top

Go:   go f()
来源：http://ljd.zdbjq.cn

Ruby: Thread.new { f }
来源：http://izz.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://gkm.jinqigfzy.top

[O02] 使用线程池
来源：http://vdd.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gto.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tfs.birdmap.top

JS:   // worker_threads 线程池
来源：http://mfp.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://bzc.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://axx.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ava.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qfs.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oix.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://ehv.zhixingplan.top

Py:   with lock: shared += 1
来源：http://qdw.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://ehf.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gur.redwolf501.top

TS:   // 同 JS
来源：http://nih.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://xbr.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hhm.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fmd.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://rfl.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://ogk.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://ojq.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mks.cucudq.cn

JS:   async function f() { await g(); }
来源：http://wku.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://soe.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oos.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pyy.52xcode.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zpw.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://pqe.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://lml.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://qyw.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zzr.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://cgb.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://izm.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lgm.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://snb.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://ouc.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xtv.shzxlz.cn

[O06] 使用进程池
来源：http://saa.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jdd.shzxlz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ypr.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://uwi.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://iep.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pur.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://spn.shuidangran.top

Ruby: // fork 块
来源：http://mcb.zhongyouzk.top

C#:   Parallel.For
来源：http://hab.cashguo.top

================================================================================
来源：http://ngx.dashuyun.cn

P. 常用工具函数
来源：http://wdz.jinqigfzy.top

================================================================================
来源：http://ecl.yonumen.top

[P01] 生成 UUID
来源：http://pqj.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://ird.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nzh.meibo888.top

JS:   crypto.randomUUID()
来源：http://dct.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://xui.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://xor.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://ach.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://yub.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://mpq.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://ksx.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tcd.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bjb.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vcs.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cjq.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vyb.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://emx.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uyd.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://twz.52xcode.cn

[P03] 生成短随机字符串
来源：http://pbx.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jop.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ybj.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ugj.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ezn.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ctk.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zrw.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://flj.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kww.nanxinkj.top

[P04] 求长度
来源：http://aom.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tyj.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://veh.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hcm.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://utn.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://xve.guannengcc.top

Go:   len(arr);  len(m)
来源：http://gxo.jyoumei.cn

Ruby: x.length;  x.size
来源：http://zdr.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://baq.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://wib.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://aiz.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xnr.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aac.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mmk.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jjq.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://vog.vehdjk.com

Ruby: a == b
来源：http://frv.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bea.jinqigufen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xnb.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oby.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://qes.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lfk.cucudq.cn

TS:   if (x == null) {}
来源：http://drg.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://urv.sjlbkw.cn

Go:   if x == nil {}
来源：http://oao.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://chh.dianchejie.cn

C#:   if (x is null) {}
来源：http://tgm.fengsongda.top

[P07] 防抖与节流
来源：http://sly.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://exm.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://qvz.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gfw.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jwx.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://znd.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oma.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://stj.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sed.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://bjc.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rph.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ees.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mjj.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hue.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wll.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://acs.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iqv.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aas.jiagoushi.top

================================================================================
来源：http://pzq.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jcd.gzhubu.top

================================================================================
来源：http://xql.yvedp.cn

[Q01] 创建表
来源：http://wtd.zhijiandao.cn

CREATE TABLE users (
来源：http://wtj.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wll.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://bfh.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://mvx.snrcjt.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://otn.zhoulong.xyz

);
来源：http://pae.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://vyv.pengpengdd.cyou

CREATE TABLE orders (
来源：http://swv.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dze.nwbrower.top

user_id INT NOT NULL,
来源：http://gde.fzhhl.top

amount DECIMAL(10, 2),
来源：http://gxy.hnxiangtu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yxc.9152youxi.cn

);
来源：http://qba.jinyuanbaomall.cn

[Q03] 增加列
来源：http://wkw.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hbb.cqqwz.cn

[Q04] 修改列类型
来源：http://ykr.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hjg.guannengcc.top

[Q05] 重命名列
来源：http://brh.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vkx.hcnkem.com

[Q06] 删除列
来源：http://ndp.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ewx.nanxinkj.top

[Q07] 删除表
来源：http://mhd.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://vqw.yj20258.top

[Q08] 创建普通索引
来源：http://dfk.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dnc.nwbrower.top

[Q09] 创建唯一索引
来源：http://goz.yangfankeji.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zjp.tianlin.xyz

[Q10] 插入单行
来源：http://ldu.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rpe.chenzaomai.com

[Q11] 一次插入多行
来源：http://inc.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://irk.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://mzj.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wlj.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uwt.vehdjk.com

[Q13] 忽略重复插入
来源：http://vny.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rbj.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://wng.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://emp.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://acm.jqgfzy.top

[Q15] 查询全部
来源：http://tdq.havefunace.top

SELECT * FROM users;
来源：http://wlx.svipenyu.cn

[Q16] 查询指定列
来源：http://pac.0kj1m.cn

SELECT id, name FROM users;
来源：http://wdr.sjlbkw.cn

[Q17] 条件查询
来源：http://lxn.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uol.iojbl.cn

[Q18] 模糊匹配
来源：http://hpc.ctjpmb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qmp.fktsv.cn

[Q19] 范围查询
来源：http://ogu.fktsv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://buh.pengpengdd.cyou

[Q20] IN 列表
来源：http://inx.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hgm.hesvh.cn

[Q21] 空值判断
来源：http://xrz.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kqs.shzxlz.cn

[Q22] 排序
来源：http://eic.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vhr.ivvv.top

[Q23] 分页
来源：http://hgi.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sde.guannengcc.top

[Q24] 去重
来源：http://rmc.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://icv.tarul.cn

[Q25] 只取前 N 条
来源：http://ojn.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nfw.svipenyu.cn

[Q26] 计数
来源：http://ppt.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://ipk.jinqigufen.top

[Q27] 条件计数
来源：http://hrv.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oxr.xziqi.cn

[Q28] 求和与平均
来源：http://tdv.jyoumei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jwo.svipenyu.cn

[Q29] 最大最小值
来源：http://qwu.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ddy.havefunace.top

[Q30] 分组统计
来源：http://wts.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qyn.ctjpmb.com

[Q31] 分组后过滤
来源：http://pov.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zaw.yvedp.cn

[Q32] 分组拼接字符串
来源：http://byg.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dtc.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ych.zhengqikj.top

[Q33] 多列分组
来源：http://xxm.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kpc.zhixingplan.top

[Q34] 每组取第一条
来源：http://kbs.quarkkingdee.top

SELECT * FROM (
来源：http://afu.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dkn.jianghu66.top

) t WHERE rn = 1;
来源：http://zlk.52xcode.cn

[Q35] 内连接
来源：http://sbu.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oze.jqgfzy.top

[Q36] 左连接
来源：http://aqz.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ucm.guowangkeji.top

[Q37] 右连接
来源：http://ago.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://csn.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://vjc.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tnb.jlsjyb.cn

[Q39] 自连接（查上下级）
来源：http://qch.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fav.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lug.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vjn.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://otu.tian-w.cn

[Q41] 多表连接
来源：http://lbw.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://jmq.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://img.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://euo.birdmap.top

[Q42] 连接条件附加过滤
来源：http://chm.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://vmw.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mpe.epnwcf.com

[Q43] 标量子查询
来源：http://bfb.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bzy.redwolf501.top


<!-- 参考信息 -->