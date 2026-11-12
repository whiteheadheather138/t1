代发 wailian999

[G10] 访问控制
来源：http://whf.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://sri.dianchejie.cn

PHP:  public / protected / private
来源：http://zfa.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://otx.shuidangran.top

TS:   public / protected / private
来源：http://qki.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://sfy.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://prj.xinyue.icu

Ruby: public / protected / private
来源：http://vjp.hnqzz.top

C#:   public / protected / private / internal
来源：http://hda.jqgufenzy.top

[G11] getter / setter
来源：http://oyj.yongpay.top

Py:   @property 与 @x.setter
来源：http://dax.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pqw.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://gcw.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://ubk.gotoacloud.top

Java: public String getName() { return name; }
来源：http://cqe.zhixingplan.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://afw.yangfankeji.com

Ruby: attr_accessor :name
来源：http://exy.redwolf501.top

C#:   public string Name { get; set; }
来源：http://jgx.fehbvm.com

[G12] 对象转字符串
来源：http://lmo.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://avr.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bgz.wangdashe.top

JS:   toString() { return this.name; }
来源：http://skb.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://bpc.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://btq.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://edm.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://abd.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://tmt.zhengqikj.top

[G13] 判断对象类型
来源：http://sks.sxryk.cn

Py:   isinstance(u, User)
来源：http://zul.xziqi.cn

PHP:  $u instanceof User
来源：http://jxo.iojbl.cn

JS:   u instanceof User
来源：http://ckk.ctjpmb.com

TS:   u instanceof User
来源：http://vle.quarkkingdee.top

Java: u instanceof User
来源：http://fvj.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ltv.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://tum.shzxlz.cn

C#:   u is User
来源：http://rmu.guowangkeji.top

[G14] 数据类 / record
来源：http://dcx.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bhn.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://akd.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vhs.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://srd.meibo888.top

Java: record User(String name, int age) {}
来源：http://zxl.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://par.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xnt.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://jhu.jlsjyb.cn

[G15] 枚举
来源：http://gvo.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fsg.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cod.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://epk.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gxv.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://ssw.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mpv.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://jyy.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://odc.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://boi.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wtf.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://xrz.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://pjg.uphjek.com

TS:   Object.entries(obj)
来源：http://jwb.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nsc.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qai.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://gpi.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://rtr.cashguo.top

================================================================================
来源：http://cdu.yuxming.cn

H. 异常与错误处理
来源：http://jhu.sxryk.cn

================================================================================
来源：http://iqd.aibaodan.cn

[H01] try / catch 基础
来源：http://svu.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xaz.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vuz.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://meq.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zco.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rjk.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vuh.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fvh.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lib.redwolf501.top

[H02] finally / ensure 收尾
来源：http://lzf.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wbq.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zig.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://adb.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://jsg.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mce.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xhr.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://swx.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vqh.dashuyun.cn

[H03] 主动抛出异常
来源：http://jtj.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://wjn.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wli.fzhhl.top

JS:   throw new Error("错误信息");
来源：http://znb.yfazqb.com

TS:   throw new Error("错误信息");
来源：http://tmq.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ezx.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dan.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vbp.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://kxp.shzxlz.cn

[H04] 自定义异常类型
来源：http://qeg.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://rru.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pbh.ydzc1.top

JS:   class MyError extends Error {}
来源：http://ugj.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://lns.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://wis.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lbg.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://got.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://vte.sysykeji.top

[H05] 捕获特定类型
来源：http://wvp.xinyue.icu

Py:   except ValueError as e:
来源：http://gsp.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tbr.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://oxh.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://svp.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://zce.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ghs.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://ztk.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xjk.dianchejie.cn

[H06] 可选值 / 空值安全访问
来源：http://jys.ybcxt.top

Py:   value = d.get("k") or default
来源：http://vde.havefunace.top

PHP:  $v = $d["k"] ?? null;
来源：http://fgq.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://akq.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mid.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://szv.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qko.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://yon.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://tfy.jqgufenzy.top

[H07] 断言
来源：http://whq.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://gme.birdmap.top

PHP:  assert($x > 0);
来源：http://fih.wangdashe.top

JS:   console.assert(x > 0);
来源：http://mja.yongpay.top

TS:   console.assert(x > 0);
来源：http://hfj.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://tth.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dqm.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://edf.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://rct.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://wwv.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://usr.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tvr.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://dvr.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jdm.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xwe.hnqzz.top

Go:   err.Error()
来源：http://xya.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://qtx.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://yhw.hnxiangtu.top

[H09] 带错误码的异常
来源：http://xlu.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zjh.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nyc.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://umq.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fkn.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hua.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ule.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://xzi.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nnb.xziqi.cn

[H10] 资源自动释放
来源：http://yot.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://afc.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://knx.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vba.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dqh.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wci.hfpthk.cn

Go:   defer f.Close()
来源：http://qfg.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yzy.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xaq.gotoacloud.top

================================================================================
来源：http://vek.hesvh.cn

I. 正则表达式
来源：http://zem.yfazqb.com

================================================================================
来源：http://fki.hywenlv.cn

[I01] 判断是否匹配
来源：http://kdt.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tud.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://trq.ybcxt.top

JS:   /\d+/.test(s)
来源：http://nyz.ybcxt.top

TS:   /\d+/.test(s)
来源：http://ssb.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fdc.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://moj.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://tgf.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mke.hfpthk.cn

[I02] 提取所有匹配
来源：http://esy.jqgufenzy.top

Py:   re.findall(r"\d+", s)
来源：http://waw.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wod.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bso.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://ebd.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://riv.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dgf.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://rdp.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cvb.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://zts.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cfy.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://idk.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lrm.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gbt.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nxq.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lpe.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tsv.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iae.52xcode.cn

[I04] 正则替换
来源：http://ebm.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xho.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ssu.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fqr.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://kcm.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://knp.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qbi.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ocd.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gez.yangfankeji.com

[I05] 按正则拆分
来源：http://ayg.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tjt.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xjr.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://kvk.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://smw.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://ljc.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ezt.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://xiu.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ikb.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hgw.shangyingyoupin.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tkp.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ddn.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hui.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jjb.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://teq.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hzq.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kpf.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gih.andypj.xyz

[I07] 忽略大小写与多行模式
来源：http://ybe.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hak.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vst.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tam.fktsv.cn

TS:   /error/gim
来源：http://qsz.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://swo.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fdw.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://bng.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qqd.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://som.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sem.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pnx.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fkm.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gme.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://nvn.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zva.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hwn.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zsb.fzhhl.top

================================================================================
来源：http://ofm.cdnleiting.top

J. 日期与时间
来源：http://szf.yj20258.top

================================================================================
来源：http://yno.haohaochexian.top

[J01] 获取当前时间
来源：http://vqq.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jdp.sxryk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://orz.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://wqb.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://xbf.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ixq.cashguo.top

Go:   time.Now()
来源：http://hgg.nwbrower.top

Ruby: Time.now
来源：http://fua.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hoa.birdmap.top

[J02] 格式化输出
来源：http://lla.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kxt.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lfd.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vba.ydzc1.top

TS:   d.toISOString()
来源：http://law.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aep.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vzb.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bov.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pwn.gogol.net.cn

[J03] 字符串解析为日期
来源：http://cuq.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wyq.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ikv.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://nqi.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://mll.xylfe.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ymn.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yej.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://owp.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kbh.tarul.cn

[J04] 时间戳与日期互转
来源：http://pia.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ery.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mwx.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jhs.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xmp.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fvu.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ptm.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://evb.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ztn.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://gwu.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://jlx.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cow.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sup.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bcw.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://olj.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zuy.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://uay.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://qsq.hywenlv.cn

[J06] 计算两时间之差
来源：http://fwx.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://fhu.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://mlq.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qmi.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pyn.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://tgo.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://sts.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://uvr.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://bma.xinyue.icu

[J07] 比较两个日期
来源：http://pvw.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://dra.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rth.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://sqr.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fvl.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ula.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xxc.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://bqa.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vwb.daxiang520.top

[J08] 提取年月日与星期
来源：http://qyh.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gpk.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pnc.ivvv.top


<!-- 参考信息 -->