代发 wailian999

TS:   public / protected / private
来源：http://kvr.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://cgj.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bdy.xylfe.cn

Ruby: public / protected / private
来源：http://mgv.xinyue.icu

C#:   public / protected / private / internal
来源：http://ahd.jyoumei.cn

[G11] getter / setter
来源：http://gyo.xuanzx.com

Py:   @property 与 @x.setter
来源：http://slq.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nzg.yongpay.top

JS:   get name() { return this._name; }
来源：http://mye.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://fdi.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://mfl.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://env.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://umn.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://prj.zhixingplan.top

[G12] 对象转字符串
来源：http://hfh.zhijiandao.cn

Py:   def __str__(self): return self.name
来源：http://stk.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://nqa.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://yra.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://iou.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://wpe.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kfj.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://cxe.chenjidiqi.icu

C#:   public override string ToString() => Name;
来源：http://xcn.hongshengwenyu.top

[G13] 判断对象类型
来源：http://xkf.shzxlz.cn

Py:   isinstance(u, User)
来源：http://fxl.cqqwz.cn

PHP:  $u instanceof User
来源：http://abm.jinqigufen.top

JS:   u instanceof User
来源：http://uyd.yonumen.top

TS:   u instanceof User
来源：http://bno.dianchejie.cn

Java: u instanceof User
来源：http://mcw.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mpa.redwolf501.top

Ruby: u.is_a?(User)
来源：http://nrg.pycfn.com

C#:   u is User
来源：http://jww.ppjwa.cn

[G14] 数据类 / record
来源：http://ksk.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hjh.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://nrm.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qdj.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://rbj.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://vtt.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://qdp.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zni.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://zzd.yj202588.top

[G15] 枚举
来源：http://yuf.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bfa.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nqn.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ino.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bnf.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://wrw.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mqo.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://iqp.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zcf.sweek.top

[G16] 对象转数组 / 字典
来源：http://zut.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sdj.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://yjk.jinqigufen.top

JS:   Object.entries(obj)
来源：http://uvy.zdbjq.cn

TS:   Object.entries(obj)
来源：http://dom.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ocj.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ody.zdbjq.cn

Ruby: obj.instance_variables
来源：http://cjj.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://oxy.cdnleiting.top

================================================================================
来源：http://ovq.andypj.xyz

H. 异常与错误处理
来源：http://tls.dashuyun.cn

================================================================================
来源：http://fhm.zhongyouzk.top

[H01] try / catch 基础
来源：http://zgy.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xcm.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dbs.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ayj.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nsi.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qyf.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xqn.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tck.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://brq.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://orf.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://nlc.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ngi.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://zop.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ejb.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tyv.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sjf.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vir.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tio.quarkkingdee.top

[H03] 主动抛出异常
来源：http://uhl.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://ldl.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mgo.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://ivg.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://dzf.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cpc.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qre.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uou.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://esj.ydzc1.top

[H04] 自定义异常类型
来源：http://mvk.meibo888.top

Py:   class MyError(Exception): pass
来源：http://gyx.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mib.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://sls.redwolf501.top

TS:   class MyError extends Error {}
来源：http://agt.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://arp.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://erh.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://nfb.guannengcc.top

C#:   class MyException : Exception {}
来源：http://vxb.zdbjq.cn

[H05] 捕获特定类型
来源：http://tns.daria6918.cn

Py:   except ValueError as e:
来源：http://qqd.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mix.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://mmd.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://qnb.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://bzm.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ira.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://qsw.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zog.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://qzr.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://svm.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kzn.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xtl.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://gfo.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vrw.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xkd.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://lvw.xziqi.cn

C#:   obj?.A?.B ?? default
来源：http://qpv.nanxuanxn.top

[H07] 断言
来源：http://wiz.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://fht.xylfe.cn

PHP:  assert($x > 0);
来源：http://tsg.xziqi.cn

JS:   console.assert(x > 0);
来源：http://wkd.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://yin.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://rec.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hwd.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://fge.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://xkh.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://izx.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://tvn.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://drg.jyoumei.cn

JS:   e.message;  e.stack
来源：http://uud.shuidangran.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mej.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nup.hammf.cn

Go:   err.Error()
来源：http://pkx.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://oad.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://fdm.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://tgn.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://btm.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://gal.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gig.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bhy.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ocy.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jfy.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://owb.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://kjx.yonumen.top

[H10] 资源自动释放
来源：http://bmf.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zuz.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://syv.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nmg.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hxd.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fab.daria6918.cn

Go:   defer f.Close()
来源：http://avk.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xzp.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xzb.birdmap.top

================================================================================
来源：http://zym.sweek.top

I. 正则表达式
来源：http://eii.sweek.top

================================================================================
来源：http://rej.yuanzhike.top

[I01] 判断是否匹配
来源：http://mmu.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://djl.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://myl.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://ddb.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://oxc.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hbu.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yha.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://apn.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gkw.yj20258.top

[I02] 提取所有匹配
来源：http://peh.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://awy.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cfl.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lux.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://dde.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://omi.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uif.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://klm.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bkc.nanxuanxn.top

[I03] 提取捕获分组
来源：http://kiv.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://htd.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xjy.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wgu.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ebh.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bsg.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fko.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zai.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sls.xuetiantiany.cn

[I04] 正则替换
来源：http://wqc.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oxz.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ila.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cms.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gin.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://mgb.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://trg.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qsj.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xpg.xuanzx.com

[I05] 按正则拆分
来源：http://eut.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xii.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bcx.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://ojm.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://nbx.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://zsj.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dqk.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://fei.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sly.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cso.zhiwuduotai.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jba.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aap.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://soa.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://did.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://utb.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vwp.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jge.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rlz.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://vqx.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hjz.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://czu.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hxp.ydzc1.top

TS:   /error/gim
来源：http://tqc.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zsq.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uua.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://hlk.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fdk.hnxiangtu.top

[I08] 贪婪与非贪婪匹配
来源：http://jca.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vsj.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbi.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oay.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dzn.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://voa.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jkt.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ahg.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tia.vqdsnc.cn

================================================================================
来源：http://dtr.chenjidiqi.icu

J. 日期与时间
来源：http://ytc.zhixingplan.top

================================================================================
来源：http://zvx.sufxvd.cn

[J01] 获取当前时间
来源：http://fhs.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pil.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qqq.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://uyf.mhx1999.top

TS:   new Date();  Date.now()
来源：http://qkb.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ytn.hnxiangtu.top

Go:   time.Now()
来源：http://hpt.gaohongyu789.top

Ruby: Time.now
来源：http://hdd.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ved.gaohongyu789.top

[J02] 格式化输出
来源：http://dlw.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nlm.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xds.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bim.gaohongyu789.top

TS:   d.toISOString()
来源：http://trj.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wob.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fji.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axk.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cxv.sweek.top

[J03] 字符串解析为日期
来源：http://hlh.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vwa.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sha.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://agq.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://yhg.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://ttq.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ozn.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://sxj.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nwy.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://tti.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iul.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dyx.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dej.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fcq.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ifd.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oqi.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rlu.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sps.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://zel.meibo888.top

Py:   now + timedelta(days=7)
来源：http://ufu.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kvf.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mbx.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vnv.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://nen.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mao.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://ovc.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fzu.sxryk.cn

[J06] 计算两时间之差
来源：http://joq.316326.xyz

Py:   (end - start).total_seconds()
来源：http://bbi.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://nfw.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qld.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lzq.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://jgz.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://bhx.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://lmb.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://hey.wangdashe.top

[J07] 比较两个日期
来源：http://kus.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://mnt.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xpc.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://ruo.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://pax.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wmb.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://txh.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://fdx.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://hwf.sxryk.cn

[J08] 提取年月日与星期
来源：http://irx.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://psc.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jvn.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pys.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nfz.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://skd.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vqu.pengpengdd.cyou


<!-- 参考信息 -->