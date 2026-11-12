代发 wailian999

[N09] 栈与队列
来源：http://uzd.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rvy.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qxx.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ugj.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nbr.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pze.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tew.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://omp.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tjx.jiagoushi.top

[N10] 链表节点定义
来源：http://crr.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rov.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vxg.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fvr.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gkb.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://cdb.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wcr.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://waa.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oet.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://tmm.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hxu.tianlin.xyz

PHP:  // 手写递归函数
来源：http://uvz.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://edn.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://phz.gotoacloud.top

Java: // 手写递归
来源：http://cgy.9152youxi.cn

Go:   // 手写递归
来源：http://yuw.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://poh.shzxlz.cn

C#:   // 手写递归
来源：http://dor.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xpk.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ydh.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cjf.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cif.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xiq.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xjl.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nlg.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qzo.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cwb.ppjwa.cn

================================================================================
来源：http://bfj.pycfn.com

O. 并发与异步
来源：http://kmr.hfpthk.cn

================================================================================
来源：http://xkr.ctjpmb.com

[O01] 启动一个线程
来源：http://qqf.vehdjk.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zac.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hsg.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wbf.zhiwuduotai.top

TS:   // 同 JS
来源：http://lms.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://wyu.pengpengdd.cyou

Go:   go f()
来源：http://dma.yj20258.top

Ruby: Thread.new { f }
来源：http://gkm.fengsongda.top

C#:   Task.Run(() => F());
来源：http://mum.jqgfzy.top

[O02] 使用线程池
来源：http://sje.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nfw.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lng.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://dis.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://iga.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vhw.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dnr.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iqn.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yen.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://gbr.jqgfzy.top

Py:   with lock: shared += 1
来源：http://lok.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://bzr.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ldq.jlsjyb.cn

TS:   // 同 JS
来源：http://nbr.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://ahj.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vyi.vqdsnc.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gqy.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://ntj.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://lvh.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://sql.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ngi.yj20258.top

JS:   async function f() { await g(); }
来源：http://kqx.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ysd.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rse.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oml.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://cbk.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://bga.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://rjj.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://gnx.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zfw.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://iuv.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://ppy.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kuy.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qiu.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://ubs.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://xfl.hcnkem.com

[O06] 使用进程池
来源：http://gek.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jrm.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vdm.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://drc.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://lly.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://crq.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hti.zycfv.cn

Ruby: // fork 块
来源：http://lvp.zhengqikj.top

C#:   Parallel.For
来源：http://gri.fengsongda.top

================================================================================
来源：http://seq.sysykeji.top

P. 常用工具函数
来源：http://uoe.tianlin.xyz

================================================================================
来源：http://sbz.ivvv.top

[P01] 生成 UUID
来源：http://hkt.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://but.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ndz.jianghu66.top

JS:   crypto.randomUUID()
来源：http://ndt.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://dkc.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://ocp.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://yys.ybcxt.top

Ruby: SecureRandom.uuid
来源：http://wgk.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://ape.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://wss.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jio.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pku.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nlv.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ppz.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ibu.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://var.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tkt.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dno.snrcjt.cn

[P03] 生成短随机字符串
来源：http://zjv.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jja.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wsm.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uvf.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tlm.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://exo.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wiy.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pye.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kcz.jinqigfzy.top

[P04] 求长度
来源：http://ums.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lmb.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fqm.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nob.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tdm.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://pqa.tanke756.top

Go:   len(arr);  len(m)
来源：http://aav.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://hgw.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nsy.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://swu.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hyl.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pov.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qka.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mly.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ciw.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://exr.shangyingyoupin.top

Ruby: a == b
来源：http://xbd.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zit.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://flw.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mjb.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://yif.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jim.pycfn.com

TS:   if (x == null) {}
来源：http://yhl.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lzq.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://toa.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fpq.yonumen.top

C#:   if (x is null) {}
来源：http://mqs.jyoumei.cn

[P07] 防抖与节流
来源：http://yhy.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cln.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://gby.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ati.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bzr.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lws.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ggj.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gze.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zlb.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://rva.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kcp.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cwx.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wpo.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://stc.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gri.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://son.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://twc.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://keb.gogol.net.cn

================================================================================
来源：http://vdi.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://elu.cucudq.cn

================================================================================
来源：http://zka.gogol.net.cn

[Q01] 创建表
来源：http://dqw.pengpengdd.cyou

CREATE TABLE users (
来源：http://ucf.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gcb.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://wwf.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://kkp.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dcm.ydzc1.top

);
来源：http://csn.smart0.xyz

[Q02] 创建带外键的表
来源：http://bfx.ydzc1.top

CREATE TABLE orders (
来源：http://pcf.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://apu.jyoumei.cn

user_id INT NOT NULL,
来源：http://ced.wangdashe.top

amount DECIMAL(10, 2),
来源：http://pvr.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vei.feifeiyinyue.top

);
来源：http://lil.mhx1999.top

[Q03] 增加列
来源：http://lfx.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aci.yj20258888.top

[Q04] 修改列类型
来源：http://hrq.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wcd.ppjwa.cn

[Q05] 重命名列
来源：http://kgf.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wmn.316326.xyz

[Q06] 删除列
来源：http://frm.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://pgc.yj202588.top

[Q07] 删除表
来源：http://mxb.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://qam.meibo888.top

[Q08] 创建普通索引
来源：http://hxe.zycfv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zrd.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://ojq.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uru.dashuyun.cn

[Q10] 插入单行
来源：http://qgx.tianlin.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xqp.hysaishi.cn

[Q11] 一次插入多行
来源：http://egn.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ndm.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://ibc.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ocb.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eqw.yj20258888.top

[Q13] 忽略重复插入
来源：http://cti.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://myy.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://tkq.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dwy.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ivq.bbcook.cn

[Q15] 查询全部
来源：http://qsb.hnxiangtu.top

SELECT * FROM users;
来源：http://uzo.bbcook.cn

[Q16] 查询指定列
来源：http://jqf.redwolf501.top

SELECT id, name FROM users;
来源：http://ccf.jyoumei.cn

[Q17] 条件查询
来源：http://vty.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qmx.nwbrower.top

[Q18] 模糊匹配
来源：http://axd.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xie.fktsv.cn

[Q19] 范围查询
来源：http://epj.jiagoushi.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oii.zycfv.cn

[Q20] IN 列表
来源：http://oxf.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tzz.cdnleiting.top

[Q21] 空值判断
来源：http://llu.hysaishi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://csx.svipenyu.cn

[Q22] 排序
来源：http://aeq.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://itu.yj202588.top

[Q23] 分页
来源：http://fcd.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qzq.yj20258.top

[Q24] 去重
来源：http://jtp.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://kil.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://ifd.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xym.zycfv.cn

[Q26] 计数
来源：http://tvp.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://zuc.fktsv.cn

[Q27] 条件计数
来源：http://ovk.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ewo.chenjidiqi.icu

[Q28] 求和与平均
来源：http://zdl.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hga.havefunace.top

[Q29] 最大最小值
来源：http://hbm.yongpay.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://usi.daria6918.cn

[Q30] 分组统计
来源：http://knl.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wym.fehbvm.com

[Q31] 分组后过滤
来源：http://psq.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jus.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://nbb.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uiz.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zez.snrcjt.cn

[Q33] 多列分组
来源：http://xdy.xziqi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ncp.yj202588.top

[Q34] 每组取第一条
来源：http://fct.snrcjt.cn

SELECT * FROM (
来源：http://sfb.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xey.quarkkingdee.top

) t WHERE rn = 1;
来源：http://ckj.hongshengwenyu.top

[Q35] 内连接
来源：http://omq.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ljf.zdbjq.cn

[Q36] 左连接
来源：http://fep.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mgb.sxryk.cn

[Q37] 右连接
来源：http://nxj.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://snl.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://yms.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://guq.yj20258.top

[Q39] 自连接（查上下级）
来源：http://ysp.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://iqs.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dkx.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pcg.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dyv.chenjidiqi.icu

[Q41] 多表连接
来源：http://ili.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ilw.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://ggc.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://fup.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://ukd.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://yku.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://psn.pycfn.com

[Q43] 标量子查询
来源：http://ckd.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://htb.316326.xyz

[Q44] IN 子查询
来源：http://vhv.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nmr.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://isx.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hsg.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://eky.ivvv.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zfi.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://vsx.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bfm.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://tgv.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rgi.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://blu.nwbrower.top

[Q49] 更新单行
来源：http://uge.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wzl.yueranfly.top

[Q50] 批量更新
来源：http://ekl.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cak.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://fjp.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://adz.fktsv.cn

[Q52] 删除指定行
来源：http://znw.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://yhb.jinqigufen.top

[Q53] 按条件删除
来源：http://aev.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kbg.xuanzx.com

[Q54] 清空表
来源：http://fvy.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://wop.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://rqk.xuetiantiany.cn


<!-- 参考信息 -->