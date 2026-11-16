代发 wailian999

[G10] 访问控制
来源：http://iwx.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://gay.jqgufenzy.top

PHP:  public / protected / private
来源：http://gep.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://kko.tarul.cn

TS:   public / protected / private
来源：http://hes.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://xsy.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://drd.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://llc.yangfankeji.com

C#:   public / protected / private / internal
来源：http://fmh.zhongyouzk.top

[G11] getter / setter
来源：http://qrg.birdmap.top

Py:   @property 与 @x.setter
来源：http://vlr.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://euc.smart0.xyz

JS:   get name() { return this._name; }
来源：http://jby.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://iwd.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://eqh.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qzt.ivvv.top

Ruby: attr_accessor :name
来源：http://vyf.zycfv.cn

C#:   public string Name { get; set; }
来源：http://mgu.yonumen.top

[G12] 对象转字符串
来源：http://hwf.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://pqt.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://xeh.316326.xyz

JS:   toString() { return this.name; }
来源：http://wjw.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://nqu.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://acs.meibo888.top

Go:   func (u User) String() string { return u.Name }
来源：http://eff.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://pkc.yj202588.top

C#:   public override string ToString() => Name;
来源：http://ppa.xziqi.cn

[G13] 判断对象类型
来源：http://xts.nanxinkj.top

Py:   isinstance(u, User)
来源：http://ijs.hnxiangtu.top

PHP:  $u instanceof User
来源：http://xtm.hysaishi.cn

JS:   u instanceof User
来源：http://xzk.fanxiaobao.xyz

TS:   u instanceof User
来源：http://nvi.daria6918.cn

Java: u instanceof User
来源：http://jrc.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fys.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://grx.fanxiaobao.xyz

C#:   u is User
来源：http://fbp.shzxlz.cn

[G14] 数据类 / record
来源：http://gmb.iojbl.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sut.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://ljb.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://djn.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://pqf.epnwcf.com

Java: record User(String name, int age) {}
来源：http://laz.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://lqk.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dfs.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://bga.hnxiangtu.top

[G15] 枚举
来源：http://brc.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gwm.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rdo.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bqi.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dip.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://kqc.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://usr.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://zky.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lbc.tarul.cn

[G16] 对象转数组 / 字典
来源：http://htq.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lit.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://wgm.yueranfly.top

JS:   Object.entries(obj)
来源：http://uyi.0kj1m.cn

TS:   Object.entries(obj)
来源：http://hms.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zqd.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jeb.redwolf501.top

Ruby: obj.instance_variables
来源：http://bml.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://lnd.epnwcf.com

================================================================================
来源：http://rde.jinqigfzy.top

H. 异常与错误处理
来源：http://dih.shuidangran.top

================================================================================
来源：http://ajd.shangyingyoupin.top

[H01] try / catch 基础
来源：http://hio.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vsr.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kjm.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gaz.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hsb.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://evd.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lzx.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kby.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ozt.gzhubu.top

[H02] finally / ensure 收尾
来源：http://rxh.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://afn.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fec.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zwe.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oce.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://srz.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gem.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cwi.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yao.andypj.xyz

[H03] 主动抛出异常
来源：http://gcg.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://hds.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oac.9152youxi.cn

JS:   throw new Error("错误信息");
来源：http://hil.yongpay.top

TS:   throw new Error("错误信息");
来源：http://ysg.meibo888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jda.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lzx.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kjm.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://rrw.gogol.net.cn

[H04] 自定义异常类型
来源：http://pma.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://kfr.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://hda.yj202588.top

JS:   class MyError extends Error {}
来源：http://teg.0kj1m.cn

TS:   class MyError extends Error {}
来源：http://ust.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://qdb.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zia.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://uei.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://fyi.kuanghao11.cn

[H05] 捕获特定类型
来源：http://gfs.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://odc.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pcy.xinyue.icu

JS:   if (e instanceof TypeError) {}
来源：http://bfb.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://uie.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://efb.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://trb.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://tuh.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ner.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://ktm.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://jlg.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://jid.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ynr.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://hjq.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tms.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://idl.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://tco.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://rlx.yanxiufei.cn

[H07] 断言
来源：http://aik.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://btx.bbcook.cn

PHP:  assert($x > 0);
来源：http://tnn.redwolf501.top

JS:   console.assert(x > 0);
来源：http://fxd.zycfv.cn

TS:   console.assert(x > 0);
来源：http://umv.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://mzy.zhoulong.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gsn.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://ldu.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://gzx.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://cog.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://qbi.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://svg.yonumen.top

JS:   e.message;  e.stack
来源：http://bdz.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dkz.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ipr.pengpengdd.cyou

Go:   err.Error()
来源：http://yor.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://tyv.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://pak.gzhubu.top

[H09] 带错误码的异常
来源：http://nwm.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qzw.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://due.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vol.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dcp.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oct.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lck.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bnv.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://dgd.dianchejie.cn

[H10] 资源自动释放
来源：http://olw.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://snx.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ssr.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pev.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xwm.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mnx.epnwcf.com

Go:   defer f.Close()
来源：http://mxw.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zup.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ekx.cdnleiting.top

================================================================================
来源：http://jtm.cqqwz.cn

I. 正则表达式
来源：http://myg.quarkkingdee.top

================================================================================
来源：http://gds.cheryme.top

[I01] 判断是否匹配
来源：http://uyt.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://isg.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fzw.cheryme.top

JS:   /\d+/.test(s)
来源：http://jjy.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://dem.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jkb.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yzv.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://yvw.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://coh.zhengqikj.top

[I02] 提取所有匹配
来源：http://xgw.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://ytr.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lbg.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nqe.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://awz.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mih.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://akm.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://ffv.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dtw.daxiang520.top

[I03] 提取捕获分组
来源：http://ism.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qpj.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gub.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jgx.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ged.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yoc.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dyz.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zzr.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ghc.hnxiangtu.top

[I04] 正则替换
来源：http://wha.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kso.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://onx.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://mpx.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lvr.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sko.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cff.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pve.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gwx.xuanzx.com

[I05] 按正则拆分
来源：http://feq.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://bdc.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fqw.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://xji.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://pjd.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://dro.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://icw.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://nol.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fdw.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yfe.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gwa.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://slt.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vjm.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mhr.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hye.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uuk.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oxa.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ebl.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://hue.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jzo.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://spl.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gtg.guowangkeji.top

TS:   /error/gim
来源：http://muk.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hub.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cxz.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://nvi.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ivr.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://vfz.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jqg.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://chr.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qse.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aez.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hfk.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://edj.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xyz.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rco.zhongyouzk.top

================================================================================
来源：http://trw.svipenyu.cn

J. 日期与时间
来源：http://kwd.yuanzhike.top

================================================================================
来源：http://axi.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://ttr.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gnh.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aeq.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://svv.cheryme.top

TS:   new Date();  Date.now()
来源：http://cqr.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bev.uphjek.com

Go:   time.Now()
来源：http://mmd.yonumen.top

Ruby: Time.now
来源：http://ruc.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://prc.cucudq.cn

[J02] 格式化输出
来源：http://gis.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nkj.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ony.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aub.ydzc1.top

TS:   d.toISOString()
来源：http://cjv.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vvc.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zlx.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jgi.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iwn.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://luv.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uvu.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vqc.yvedp.cn

JS:   new Date("2024-01-02")
来源：http://agd.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://amm.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://brn.jinghuilouyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zcn.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://nwv.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://osq.smart0.xyz

[J04] 时间戳与日期互转
来源：http://sev.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mth.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sfo.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kgz.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dvz.pengpengdd.cyou

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cid.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sdp.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fld.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ozt.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://fcw.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://htm.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lst.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xxv.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bei.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://yqr.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zrl.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://ede.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://xje.jinqigfzy.top

[J06] 计算两时间之差
来源：http://zsq.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://tif.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://zpp.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://caj.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gwl.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://sab.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://cbh.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://mgj.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://dis.sxryk.cn

[J07] 比较两个日期
来源：http://jav.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://eyg.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bao.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://wja.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kiz.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fzs.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fqb.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://osj.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://dok.9152youxi.cn

[J08] 提取年月日与星期
来源：http://rry.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lgo.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xdj.yanxiufei.cn


<!-- 参考信息 -->