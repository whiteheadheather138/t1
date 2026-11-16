代发 wailian999

Java: interface Shape { double area(); }
来源：http://yux.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://vmm.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://crt.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://ish.uphjek.com

[G10] 访问控制
来源：http://rcj.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://zjg.zhixingplan.top

PHP:  public / protected / private
来源：http://zkt.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://wmi.shangyingyoupin.top

TS:   public / protected / private
来源：http://tqf.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://qzr.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://wui.shuidangran.top

Ruby: public / protected / private
来源：http://oyu.hesvh.cn

C#:   public / protected / private / internal
来源：http://ooe.hywenlv.cn

[G11] getter / setter
来源：http://pan.fehbvm.com

Py:   @property 与 @x.setter
来源：http://xhn.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wml.fengsongda.top

JS:   get name() { return this._name; }
来源：http://ccc.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://ugp.ybcxt.top

Java: public String getName() { return name; }
来源：http://sru.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://pko.daxiang520.top

Ruby: attr_accessor :name
来源：http://ieu.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://omx.cashguo.top

[G12] 对象转字符串
来源：http://fdt.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://jdw.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://wnp.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://mcj.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://ecg.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://wmu.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://vdf.yuxming.cn

Ruby: def to_s; @name; end
来源：http://bwa.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://qol.havefunace.top

[G13] 判断对象类型
来源：http://vhu.fengsongda.top

Py:   isinstance(u, User)
来源：http://lpc.zhengqikj.top

PHP:  $u instanceof User
来源：http://pdd.fzhhl.top

JS:   u instanceof User
来源：http://uut.zhiwuduotai.top

TS:   u instanceof User
来源：http://lpw.yonumen.top

Java: u instanceof User
来源：http://zyw.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jgq.cheryme.top

Ruby: u.is_a?(User)
来源：http://ili.zycfv.cn

C#:   u is User
来源：http://bmw.zhengqikj.top

[G14] 数据类 / record
来源：http://tgb.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ive.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://uoj.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://dia.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://tyk.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://aei.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://uml.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zdk.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://dnq.jinghuilouyu.cn

[G15] 枚举
来源：http://ybx.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mrb.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ivz.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iod.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iak.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://nyk.birdmap.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://emi.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://nam.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://urh.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://iht.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pqw.316326.xyz

PHP:  get_object_vars($obj);
来源：http://feg.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://wxi.tanke756.top

TS:   Object.entries(obj)
来源：http://xih.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zjn.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zrx.chenlongwang.top

Ruby: obj.instance_variables
来源：http://jdj.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://hnn.hammf.cn

================================================================================
来源：http://ulf.guowangkeji.top

H. 异常与错误处理
来源：http://kgt.cheryme.top

================================================================================
来源：http://txl.tian-w.cn

[H01] try / catch 基础
来源：http://qct.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://veq.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cnb.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xhx.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://svx.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wrv.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cni.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ctp.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mwo.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://myz.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://stm.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://fzl.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uza.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wnx.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://llj.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ajk.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jmj.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qgt.pycfn.com

[H03] 主动抛出异常
来源：http://msd.ydzc1.top

Py:   raise ValueError("错误信息")
来源：http://rba.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ocu.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://nqr.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://hwt.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gcs.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://att.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xif.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ype.sjlbkw.cn

[H04] 自定义异常类型
来源：http://nfd.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://qrl.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gne.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://avz.cucudq.cn

TS:   class MyError extends Error {}
来源：http://frh.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://afh.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rsh.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://rms.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://alg.ybcxt.top

[H05] 捕获特定类型
来源：http://nye.iojbl.cn

Py:   except ValueError as e:
来源：http://bbm.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cfb.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://tkl.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://xai.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://pjh.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uir.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://inv.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://urz.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://kim.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://lzj.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ryu.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://xjt.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://pjb.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zre.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gzh.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://ygj.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://zif.pengpengdd.cyou

[H07] 断言
来源：http://ccx.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://tsg.zhiwuduotai.top

PHP:  assert($x > 0);
来源：http://oqg.fanxiaobao.xyz

JS:   console.assert(x > 0);
来源：http://hdd.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://aef.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://dnc.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://klt.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jzh.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://uct.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://pmg.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://par.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yge.chenlongwang.top

JS:   e.message;  e.stack
来源：http://tni.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yst.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lwr.ybcxt.top

Go:   err.Error()
来源：http://gwa.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://exh.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://sui.aibaodan.cn

[H09] 带错误码的异常
来源：http://tfl.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://heu.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xaw.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://enu.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mxy.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fyf.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bft.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://zdr.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lhx.zdqjudy.top

[H10] 资源自动释放
来源：http://hnx.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://myq.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hcv.tianlin.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pgz.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iyq.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wju.dianchejie.cn

Go:   defer f.Close()
来源：http://uin.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xbd.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bgd.haohaochexian.top

================================================================================
来源：http://qpq.zhixingplan.top

I. 正则表达式
来源：http://ngn.quarkkingdee.top

================================================================================
来源：http://ngx.shuidangran.top

[I01] 判断是否匹配
来源：http://gxv.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ito.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zcb.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://eiu.hesvh.cn

TS:   /\d+/.test(s)
来源：http://xad.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ijq.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bix.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://imi.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jqo.snrcjt.cn

[I02] 提取所有匹配
来源：http://uje.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://taf.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jvy.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lfe.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://gkf.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://khs.tarul.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hih.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://rtz.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uvw.jinqigfzy.top

[I03] 提取捕获分组
来源：http://jvd.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ycg.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lhc.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pkh.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wua.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kpf.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ykr.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kpo.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://erb.hfpthk.cn

[I04] 正则替换
来源：http://dja.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wch.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jpn.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://aic.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://iqj.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://sdd.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://cgp.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://sxd.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://igz.pycfn.com

[I05] 按正则拆分
来源：http://vmh.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nhk.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://laz.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://qdr.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://txy.hywenlv.cn

Java: s.split("\\s*,\\s*")
来源：http://uln.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sob.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://zvh.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jhu.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://exa.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hef.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hqm.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nyu.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jsc.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zjh.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ydb.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bfu.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xjo.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://glr.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mfh.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wht.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qql.redwolf501.top

TS:   /error/gim
来源：http://ynd.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bzd.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://poh.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://fow.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zwn.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://tpr.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nqx.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rdl.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nsg.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ukk.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yvj.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vft.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pag.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wko.shuidangran.top

================================================================================
来源：http://osb.ppjwa.cn

J. 日期与时间
来源：http://swv.jinqigufen.top

================================================================================
来源：http://ktv.cheryme.top

[J01] 获取当前时间
来源：http://dgl.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://huo.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lhh.aizwys.cn

JS:   new Date();  Date.now()
来源：http://rzk.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://kli.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fpx.jlsjyb.cn

Go:   time.Now()
来源：http://efa.zhiwuduotai.top

Ruby: Time.now
来源：http://eis.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nie.yueranfly.top

[J02] 格式化输出
来源：http://oof.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fbm.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rzh.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oia.xuanzx.com

TS:   d.toISOString()
来源：http://gle.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sto.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yfa.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rmy.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://czd.jqgfzy.top

[J03] 字符串解析为日期
来源：http://bld.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wuz.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lbo.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://biw.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://kcv.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://oyp.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://clm.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://cal.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jdo.fengsongda.top

[J04] 时间戳与日期互转
来源：http://odz.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uaz.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vvt.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nuh.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pul.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lyt.kuanghao11.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cax.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hys.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://acg.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://yyq.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://tog.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pow.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bfl.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://afg.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ymx.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tje.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://oir.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://jxb.hysaishi.cn

[J06] 计算两时间之差
来源：http://hwr.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://hem.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://mks.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oui.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mla.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eeo.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://hqn.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://czz.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://ywq.gogol.net.cn

[J07] 比较两个日期
来源：http://wkt.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://vnw.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tvg.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://uzh.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://uxc.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nhd.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hsw.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://czl.iojbl.cn


<!-- 参考信息 -->