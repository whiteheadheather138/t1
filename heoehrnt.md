代发 wailian999

[G10] 访问控制
来源：http://kjy.zdbjq.cn

Py:   约定 _protected / __private（不强制）
来源：http://xsy.kuanghao11.cn

PHP:  public / protected / private
来源：http://bzm.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://uys.chenjidiqi.icu

TS:   public / protected / private
来源：http://kae.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://mwi.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://oai.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://nxj.52xcode.cn

C#:   public / protected / private / internal
来源：http://fkx.meibo888.top

[G11] getter / setter
来源：http://cmf.fengsongda.top

Py:   @property 与 @x.setter
来源：http://yny.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jjy.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://qul.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://yog.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://loh.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nql.sysykeji.top

Ruby: attr_accessor :name
来源：http://nkl.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://mgx.uphjek.com

[G12] 对象转字符串
来源：http://hvd.ivvv.top

Py:   def __str__(self): return self.name
来源：http://mco.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sff.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://ivo.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://vxr.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://ucp.yangfankeji.com

Go:   func (u User) String() string { return u.Name }
来源：http://cgt.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://fnu.yonumen.top

C#:   public override string ToString() => Name;
来源：http://oer.jiagoushi.top

[G13] 判断对象类型
来源：http://tvb.sxryk.cn

Py:   isinstance(u, User)
来源：http://pyx.316326.xyz

PHP:  $u instanceof User
来源：http://vhb.sysykeji.top

JS:   u instanceof User
来源：http://xvx.meibo888.top

TS:   u instanceof User
来源：http://elo.nanxinkj.top

Java: u instanceof User
来源：http://otv.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rzi.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://xlt.zycfv.cn

C#:   u is User
来源：http://jxx.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://dwr.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tue.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://kez.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://avd.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://hny.shuidangran.top

Java: record User(String name, int age) {}
来源：http://myx.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://dpp.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://imk.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://bwb.0kj1m.cn

[G15] 枚举
来源：http://wzf.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vls.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://skf.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ucn.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hae.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://uie.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cmv.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://dnb.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://emf.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://qkv.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qle.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://ajy.jqgfzy.top

JS:   Object.entries(obj)
来源：http://gys.zhengqikj.top

TS:   Object.entries(obj)
来源：http://yly.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gyu.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gvk.sysykeji.top

Ruby: obj.instance_variables
来源：http://sdp.shanyushiyangtech.top

C#:   // 用反射或 System.Text.Json
来源：http://ryy.fzhhl.top

================================================================================
来源：http://xls.nanxuanxn.top

H. 异常与错误处理
来源：http://kze.chenlongwang.top

================================================================================
来源：http://oex.chenjidiqi.icu

[H01] try / catch 基础
来源：http://bzq.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oqs.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cbj.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sup.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hdu.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://egi.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aod.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ojw.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dsb.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://ttp.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://vvf.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bgt.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://pkg.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://exr.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xks.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://byn.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://kih.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://luz.jqgfzy.top

[H03] 主动抛出异常
来源：http://oqs.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://wox.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xvn.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://swm.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://zlf.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rgz.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kbl.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ijt.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://znk.aibaodan.cn

[H04] 自定义异常类型
来源：http://nkp.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://ckw.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://mkv.guannengcc.top

JS:   class MyError extends Error {}
来源：http://krx.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://lmw.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://wxt.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xgy.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://nvs.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://swx.jyoumei.cn

[H05] 捕获特定类型
来源：http://dta.ybcxt.top

Py:   except ValueError as e:
来源：http://had.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dxe.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://ayp.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://jua.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://buq.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yze.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://grg.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cve.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://tlc.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://vsb.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tvv.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://udj.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ggu.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tqp.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dzp.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://zzk.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://vtb.hfpthk.cn

[H07] 断言
来源：http://kqd.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://qua.nanxinkj.top

PHP:  assert($x > 0);
来源：http://dog.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://ghr.zycfv.cn

TS:   console.assert(x > 0);
来源：http://kuh.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://xfs.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rtr.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://icx.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://vqu.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://pdl.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ndg.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gts.dashuyun.cn

JS:   e.message;  e.stack
来源：http://hak.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://xwd.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jne.fzhhl.top

Go:   err.Error()
来源：http://fmf.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://zqu.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://fxi.fehbvm.com

[H09] 带错误码的异常
来源：http://uce.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oia.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fvz.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iay.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zit.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rhi.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vzy.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://bdi.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jim.tanke756.top

[H10] 资源自动释放
来源：http://nyb.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jip.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nph.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uvi.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ana.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nur.zdqjudy.top

Go:   defer f.Close()
来源：http://sgx.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uxl.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rce.52xcode.cn

================================================================================
来源：http://lhq.vehdjk.com

I. 正则表达式
来源：http://nwk.jinghuilouyu.cn

================================================================================
来源：http://thq.daxiang520.top

[I01] 判断是否匹配
来源：http://zcu.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jud.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://gpp.redwolf501.top

JS:   /\d+/.test(s)
来源：http://lnn.hnqzz.top

TS:   /\d+/.test(s)
来源：http://ipd.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dtt.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kcx.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://eya.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xmk.chenlongwang.top

[I02] 提取所有匹配
来源：http://uix.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://tal.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pag.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ong.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://qso.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fnh.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://csd.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://ftd.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ihd.bjfxy.top

[I03] 提取捕获分组
来源：http://rdu.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qvj.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yyz.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://und.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yew.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://abp.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kth.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jkm.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kyq.zhiwuduotai.top

[I04] 正则替换
来源：http://jif.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bqj.sjlbkw.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eta.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://der.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://krr.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://rpu.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uvi.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kwu.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cjy.epnwcf.com

[I05] 按正则拆分
来源：http://zpw.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gvk.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://suh.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://wrz.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://rlh.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://pmb.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iyw.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ojy.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bil.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cly.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bqd.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fkj.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://umv.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qra.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pib.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lfd.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rij.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xui.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://xdv.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://onh.fktsv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nzg.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://enh.yj202588.top

TS:   /error/gim
来源：http://tit.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wro.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pgr.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://uii.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://efn.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://hlj.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rwg.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xsd.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lml.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wyf.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fuo.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uxa.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ybf.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tmp.snrcjt.cn

================================================================================
来源：http://ipk.yj20258888.top

J. 日期与时间
来源：http://sbl.svipenyu.cn

================================================================================
来源：http://tkf.smart0.xyz

[J01] 获取当前时间
来源：http://mew.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yar.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xhy.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://ahi.jianghu66.top

TS:   new Date();  Date.now()
来源：http://vjl.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dau.sjlbkw.cn

Go:   time.Now()
来源：http://rnt.ppjwa.cn

Ruby: Time.now
来源：http://mpe.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oia.bjfxy.top

[J02] 格式化输出
来源：http://cxa.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rdh.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tsa.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://krc.zdbjq.cn

TS:   d.toISOString()
来源：http://zvi.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rtw.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lbm.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uas.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nql.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://pfg.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jdm.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pxt.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://llw.xuetiantiany.cn

TS:   new Date("2024-01-02")
来源：http://zdb.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://dsn.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gfp.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://djs.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vde.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://wxt.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lfo.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dxv.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dcq.316326.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://agy.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://chm.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zsb.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cxs.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tce.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://fuf.ivvv.top

Py:   now + timedelta(days=7)
来源：http://ljg.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rog.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fhl.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cys.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://llk.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sxs.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://ipb.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://aww.shzxlz.cn

[J06] 计算两时间之差
来源：http://uns.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://wct.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://ycq.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hrs.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://usk.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://cah.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://woa.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://pwz.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://qai.hysaishi.cn

[J07] 比较两个日期
来源：http://ijv.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://omy.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lad.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kwy.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://efq.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://irj.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://inw.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://xsj.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://ncy.jinghuilouyu.cn

[J08] 提取年月日与星期
来源：http://xmm.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xje.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pok.guowangkeji.top


<!-- 参考信息 -->