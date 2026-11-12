代发 wailian999

[G10] 访问控制
来源：http://pza.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://hto.yj20258.top

PHP:  public / protected / private
来源：http://wmc.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://zux.gaohongyu789.top

TS:   public / protected / private
来源：http://rbn.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://mfa.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://exc.sjlbkw.cn

Ruby: public / protected / private
来源：http://eiy.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://mve.zdqjudy.top

[G11] getter / setter
来源：http://cpr.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://yrt.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iij.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://cqu.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://flt.jyoumei.cn

Java: public String getName() { return name; }
来源：http://nmk.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://why.sufxvd.cn

Ruby: attr_accessor :name
来源：http://tjt.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://cwp.hammf.cn

[G12] 对象转字符串
来源：http://vva.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://nfe.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ktt.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://tbd.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://pmn.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://ylb.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://fup.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://mkb.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://ppx.hcnkem.com

[G13] 判断对象类型
来源：http://srt.fehbvm.com

Py:   isinstance(u, User)
来源：http://aqs.redwolf501.top

PHP:  $u instanceof User
来源：http://zim.yvedp.cn

JS:   u instanceof User
来源：http://utk.sxryk.cn

TS:   u instanceof User
来源：http://syv.kuanghao11.cn

Java: u instanceof User
来源：http://bku.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vwv.sxryk.cn

Ruby: u.is_a?(User)
来源：http://ezq.xuetiantiany.cn

C#:   u is User
来源：http://ugx.fengsongda.top

[G14] 数据类 / record
来源：http://rfb.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ukx.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://tqf.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://daf.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://wsf.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://wkz.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://djb.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hlz.ivvv.top

C#:   record User(string Name, int Age);
来源：http://oxn.birdmap.top

[G15] 枚举
来源：http://opd.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ctr.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vvx.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vkk.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xpf.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://eef.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jhv.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://sog.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rzl.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://rbk.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://abq.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://qbg.cheryme.top

JS:   Object.entries(obj)
来源：http://wtp.9152youxi.cn

TS:   Object.entries(obj)
来源：http://qud.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bga.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://xdk.yangfankeji.com

Ruby: obj.instance_variables
来源：http://fot.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://ooc.xziqi.cn

================================================================================
来源：http://ibq.316326.xyz

H. 异常与错误处理
来源：http://sfe.zhoulong.xyz

================================================================================
来源：http://nsw.fzhhl.top

[H01] try / catch 基础
来源：http://zkx.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jxe.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kql.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wjo.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pnm.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lbf.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dsa.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://csa.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ngk.hesvh.cn

[H02] finally / ensure 收尾
来源：http://kur.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://myg.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://xut.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uak.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gkg.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://arv.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zrg.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://zcr.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lqj.uphjek.com

[H03] 主动抛出异常
来源：http://ark.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://gbz.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xmo.yongpay.top

JS:   throw new Error("错误信息");
来源：http://kot.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://riv.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xxb.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mia.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://piu.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://rvr.jlsjyb.cn

[H04] 自定义异常类型
来源：http://dtj.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://lyk.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://gns.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://wjc.52xcode.cn

TS:   class MyError extends Error {}
来源：http://rmz.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://sci.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wca.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://tnr.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://feo.jinqigufen.top

[H05] 捕获特定类型
来源：http://qjs.andypj.xyz

Py:   except ValueError as e:
来源：http://fhz.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ilu.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://xcq.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://ngq.wangshuangyany.cn

Java: catch (IOException | SQLException e) {}
来源：http://tec.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://anw.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://ast.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vnc.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://meu.aizwys.cn

Py:   value = d.get("k") or default
来源：http://lwd.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ohq.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://qcx.yanxiufei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qdm.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mcn.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://kdg.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://myg.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://kek.316326.xyz

[H07] 断言
来源：http://xua.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://elp.smart0.xyz

PHP:  assert($x > 0);
来源：http://jam.tanke756.top

JS:   console.assert(x > 0);
来源：http://ayg.cashguo.top

TS:   console.assert(x > 0);
来源：http://ulf.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://vaw.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rtn.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://hyx.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://ydk.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://zlv.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://gry.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bkt.chenlongwang.top

JS:   e.message;  e.stack
来源：http://wfu.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wmw.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ysr.zdbjq.cn

Go:   err.Error()
来源：http://yqn.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://tbg.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://qvu.ehwqpu.com

[H09] 带错误码的异常
来源：http://tsr.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cvo.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zrq.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yic.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rwu.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mai.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ndg.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://dsr.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sjp.chenzaomai.com

[H10] 资源自动释放
来源：http://wag.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://eow.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jnu.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vgj.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kvy.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://whi.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://fuc.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lut.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xya.hysaishi.cn

================================================================================
来源：http://ffg.jinyuanbaomall.cn

I. 正则表达式
来源：http://jgo.316326.xyz

================================================================================
来源：http://kek.yj202588.top

[I01] 判断是否匹配
来源：http://woz.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kch.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xve.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://nmw.redwolf501.top

TS:   /\d+/.test(s)
来源：http://idg.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://slp.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hhf.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://vma.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hbs.nanxuanxn.top

[I02] 提取所有匹配
来源：http://ipz.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://eeh.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gbi.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://doq.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://awj.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gad.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vzv.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://yfl.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ezx.jyoumei.cn

[I03] 提取捕获分组
来源：http://ppf.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rox.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lep.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tfj.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xdo.jlsjyb.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://plf.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://syf.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uzf.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uck.uphjek.com

[I04] 正则替换
来源：http://hbd.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eku.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://moh.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://mmk.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://qvf.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://szk.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://afm.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dpt.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vnm.havefunace.top

[I05] 按正则拆分
来源：http://xsq.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://woe.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ryg.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://rey.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://xxr.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://hdy.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ixe.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xed.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sed.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xas.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ibl.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vut.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jpg.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lrf.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hzr.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://khl.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rkj.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://any.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://jxx.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vtb.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yyi.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jyg.feifeiyinyue.top

TS:   /error/gim
来源：http://swg.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rxi.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nsz.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://qgj.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jzp.hnxiangtu.top

[I08] 贪婪与非贪婪匹配
来源：http://kwu.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://izm.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vgf.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xrm.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vsg.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bgr.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://txt.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rlh.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fyv.yvedp.cn

================================================================================
来源：http://tbz.chenzaomai.com

J. 日期与时间
来源：http://gzw.sxryk.cn

================================================================================
来源：http://qib.sxryk.cn

[J01] 获取当前时间
来源：http://gji.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yui.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://odl.zhaomingkeji.xyz

JS:   new Date();  Date.now()
来源：http://bsw.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://lxk.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tie.fehbvm.com

Go:   time.Now()
来源：http://pmr.gotoacloud.top

Ruby: Time.now
来源：http://vkf.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xsz.nanxinkj.top

[J02] 格式化输出
来源：http://aus.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ubz.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gqe.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zef.snrcjt.cn

TS:   d.toISOString()
来源：http://oqn.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cjy.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wec.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tzf.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vvf.bjfxy.top

[J03] 字符串解析为日期
来源：http://jim.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fvk.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ref.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://yxc.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://kxp.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://zft.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vmf.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://ukj.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://edz.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://olz.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cyb.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nox.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ggm.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://sxe.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tdx.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wcl.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvd.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gnv.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://tnn.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://aci.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wwc.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uxe.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kkr.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://mvy.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dbw.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://sau.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://mbv.hesvh.cn

[J06] 计算两时间之差
来源：http://kcf.tarul.cn

Py:   (end - start).total_seconds()
来源：http://osi.xziqi.cn

PHP:  $end->diff($start)->days;
来源：http://caa.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ihv.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybn.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://swj.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://zfa.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://vqh.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://jqk.nanxinkj.top

[J07] 比较两个日期
来源：http://ahd.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://cde.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hjd.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://puo.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://rwe.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wsu.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uan.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://mpq.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://mav.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://ztc.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vub.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qay.kuanghao11.cn


<!-- 参考信息 -->