代发 wailian999

[Q80] 字符串截取
来源：http://sce.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oji.hywenlv.cn

[Q81] 字符串替换
来源：http://kgu.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dph.316326.xyz

[Q82] 字符长度与字节长度
来源：http://mvs.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qrv.sysykeji.top

[Q83] 大小写转换
来源：http://hwt.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://djb.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://hnv.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://vcy.ivvv.top

[Q85] 数值取整
来源：http://rwn.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zpk.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://lbl.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://glb.yfazqb.com

[Q87] JSON 字段做条件
来源：http://jde.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nzb.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://hwj.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wew.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gbd.tarul.cn

[Q89] 判断表是否存在
来源：http://rwj.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://neq.nwbrower.top

[Q90] 生成序号列
来源：http://ghm.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lmi.vqdsnc.cn

================================================================================
来源：http://gll.tian-w.cn

R. Bash 专题
来源：http://yza.hesvh.cn

================================================================================
来源：http://jst.yvedp.cn

[R01] shebang 与严格模式
来源：http://ruy.hnxiangtu.top

#!/usr/bin/env bash
来源：http://mpe.hywenlv.cn

set -euo pipefail
来源：http://ubz.hcnkem.com

[R02] 变量赋值与使用
来源：http://rwo.cdnleiting.top

name="Tom"; echo "$name"
来源：http://kft.c1oappe.top

[R03] 只读变量
来源：http://vin.epnwcf.com

readonly PI=3.14
来源：http://hwg.snrcjt.cn

[R04] 位置参数
来源：http://uab.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://izr.ehwqpu.com

[R05] 参数默认值
来源：http://tlf.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://prk.bbcook.cn

[R06] 判断命令是否存在
来源：http://vsa.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://puf.chenjidiqi.icu

[R07] if 判断文件
来源：http://qin.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qcj.daxiang520.top

[R08] 数值比较
来源：http://fio.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://trs.xinyue.icu

[R09] 字符串比较
来源：http://qda.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xci.svipenyu.cn

[R10] 正则匹配
来源：http://tyj.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qjn.cheryme.top

[R11] case 多分支
来源：http://hce.yfazqb.com

case "$1" in
来源：http://jyc.nwbrower.top

start) echo "启动" ;;
来源：http://usk.epnwcf.com

stop)  echo "停止" ;;
来源：http://ewk.yueranfly.top

*)     echo "未知命令" ;;
来源：http://uqk.hfpthk.cn

esac
来源：http://zmk.316326.xyz

[R12] for 遍历文件
来源：http://zve.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://uph.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://cgk.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://fvr.cashguo.top

[R14] C 风格 for
来源：http://yoq.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hck.uphjek.com

[R15] while 逐行读文件
来源：http://cyj.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gyk.jianghu66.top

[R16] until 等待条件
来源：http://lns.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yef.ctjpmb.com

[R17] 数组定义与取值
来源：http://ytj.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oqg.xuetiantiany.cn

[R18] 遍历数组
来源：http://rdw.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uuy.jinqigufen.top

[R19] 数组长度
来源：http://aaj.sufxvd.cn

echo "${#arr[@]}"
来源：http://zod.gogol.net.cn

[R20] 关联数组（字典）
来源：http://hbp.havefunace.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hcd.zycfv.cn

[R21] 字符串长度
来源：http://pcr.smart0.xyz

echo "${#s}"
来源：http://yhj.vqdsnc.cn

[R22] 截取子串
来源：http://erf.xuanzx.com

echo "${s:0:5}"
来源：http://csb.shzxlz.cn

[R23] 字符串替换
来源：http://qxf.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cxj.cdnleiting.top

[R24] 大小写转换
来源：http://gde.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://rzu.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://nfj.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jpt.jianghu66.top

[R26] 命令替换
来源：http://kqw.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://kwy.hcnkem.com

[R27] 算术展开
来源：http://alk.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://wfn.vqdsnc.cn

[R28] 浮点运算
来源：http://gfb.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://nmi.ydzc1.top

[R29] 定义函数
来源：http://udy.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xih.sysykeji.top

[R30] 函数返回状态码
来源：http://wue.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://vlj.chenlongwang.top

[R31] 局部变量
来源：http://xsi.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://fxd.jlsjyb.cn

[R32] 参数个数校验
来源：http://ecq.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pnv.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://lal.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zek.yuanzhike.top

[R34] 退出时清理
来源：http://mbg.nanxuanxn.top

trap 'rm -f "$tmp"' EXIT
来源：http://ypc.dashuyun.cn

[R35] 后台执行并等待
来源：http://xop.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://odw.c1oappe.top

[R36] 并发执行多个任务
来源：http://hbn.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://seb.shuidangran.top

[R37] 把输出赋给变量
来源：http://bom.smart0.xyz

files=$(ls -1)
来源：http://vxv.yuxming.cn

[R38] 管道串联
来源：http://mnv.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://hkp.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://jfs.316326.xyz

cmd > out.log 2>&1
来源：http://pst.aibaodan.cn

[R40] 追加写日志
来源：http://hcz.dashuyun.cn

echo "log" >> out.log
来源：http://abi.yvedp.cn

[R41] 丢弃输出
来源：http://xea.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://dxv.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://acj.uphjek.com

wc -l < a.txt
来源：http://bdd.yuanzhike.top

[R43] 按名字查找文件
来源：http://czl.nanxuanxn.top

find . -name "*.log" -type f
来源：http://yuw.fehbvm.com

[R44] 按修改时间查找
来源：http://eaj.redwolf501.top

find . -mtime -7 -type f
来源：http://dhu.pengpengdd.cyou

[R45] 批量删除
来源：http://cbz.meibo888.top

find . -name "*.tmp" -delete
来源：http://tci.yj202588.top

[R46] 递归替换文件内容
来源：http://yed.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wfo.yj20258888.top

[R47] sed 单行替换
来源：http://qwz.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mkh.jianghu66.top

[R48] awk 取指定列
来源：http://jfw.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://gyv.zhoulong.xyz

[R49] awk 带条件
来源：http://anz.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fdm.nanxinkj.top

[R50] awk 求和
来源：http://che.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://luh.jianghu66.top

[R51] 排序去重取前几
来源：http://zjm.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pjd.0kj1m.cn

[R52] 统计行数
来源：http://hhc.cdnleiting.top

wc -l a.txt
来源：http://aiz.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://diu.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://frs.ydjk.org.cn

[R54] 比较两个文件
来源：http://gmw.ydzc1.top

diff a.txt b.txt
来源：http://bey.hesvh.cn

[R55] 压缩与解压
来源：http://nlm.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nsg.gaohongyu789.top

[R56] 远程拷贝
来源：http://kch.yvedp.cn

scp file user@host:/path/
来源：http://jbt.ivvv.top

[R57] 远程执行命令
来源：http://qza.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://zjb.fzhhl.top

[R58] 下载文件
来源：http://pjw.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jax.ydjk.org.cn

[R59] 发 POST JSON
来源：http://opp.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://swa.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://dkt.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ped.vehdjk.com

[R61] 磁盘占用
来源：http://uvy.xinyue.icu

df -h;  du -sh *
来源：http://xpt.jinqigufen.top

[R62] 找最占空间的文件
来源：http://wev.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://uzr.andypj.xyz

[R63] 内存与进程
来源：http://lix.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://igo.jyoumei.cn

[R64] 结束进程
来源：http://zrw.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://vwv.yj202588.top

[R65] 查看端口占用
来源：http://aqk.svipenyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://imc.shangyingyoupin.top

[R66] 定时任务
来源：http://jpe.xziqi.cn

crontab -e;  crontab -l
来源：http://uyy.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://pou.fengsongda.top

openssl rand -hex 16
来源：http://ohu.hesvh.cn

[R68] 计算文件校验值
来源：http://ric.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://ial.havefunace.top

[R69] 生成随机密码
来源：http://rop.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://wbp.epnwcf.com

[R70] 时间戳与互转
来源：http://msc.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://xak.sysykeji.top

[R71] 日期格式化
来源：http://wgt.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sot.gaohongyu789.top

[R72] 等待端口就绪
来源：http://hwy.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qlh.iojbl.cn

[R73] 分割大日志
来源：http://otb.yonumen.top

split -l 1000 big.log part_
来源：http://fcy.gaohongyu789.top

[R74] 批量重命名
来源：http://zdl.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fpa.fktsv.cn

[R75] 导出环境变量
来源：http://yum.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://xlf.zdbjq.cn

[R76] 使用临时文件
来源：http://caj.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sqx.nwbrower.top

[R77] 读取用户输入
来源：http://mxh.cqqwz.cn

read -rp "请输入: " ans
来源：http://xlq.jiagoushi.top

[R78] 交互式菜单
来源：http://sxn.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://shn.hcnkem.com

[R79] 解析命令行选项
来源：http://oro.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pga.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://fjx.mhx1999.top

time ./run.sh
来源：http://ovp.ywan-chungtsiang.top

================================================================================
来源：http://qzq.guannengcc.top

S. C / C++ 专题
来源：http://vkk.shanyushiyangtech.top

================================================================================
来源：http://xex.quarkkingdee.top

[S01] C：Hello World
来源：http://mgw.yangfankeji.com

#include <stdio.h>
来源：http://pfx.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hbu.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://piy.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://lma.meibo888.top

[S03] C：读入整数
来源：http://quo.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://hlt.dianchejie.cn

[S04] C：字符串复制
来源：http://meu.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zcf.chenlongwang.top

[S05] C：字符串长度
来源：http://ecp.meibo888.top

strlen(s)
来源：http://asf.gotoacloud.top

[S06] C：字符串比较
来源：http://wbv.guannengcc.top

strcmp(a, b) == 0
来源：http://tjc.xuanzx.com

[S07] C：数组遍历求和
来源：http://vwu.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zzj.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://rls.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ahq.sweek.top

[S09] C：结构体定义与初始化
来源：http://hxx.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ndx.meibo888.top

[S10] C：指针与解引用
来源：http://sep.bjfxy.top

int *p = &a;  *p = 5;
来源：http://dbt.xziqi.cn

[S11] C：逐行读文件
来源：http://nmh.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://vmm.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xlc.dianchejie.cn

fclose(f);
来源：http://yzg.ydzc1.top

[S12] C：写文件
来源：http://qhw.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kgg.epnwcf.com

[S13] C：宏定义
来源：http://tuh.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://srh.nanxuanxn.top

[S14] C：枚举
来源：http://stg.yj20258.top

enum Color { RED, GREEN, BLUE };
来源：http://yod.snrcjt.cn

[S15] C：类型转换
来源：http://bnr.xuetiantiany.cn

(double) a / b
来源：http://cjk.zhoulong.xyz

[S16] C：位操作置位
来源：http://vms.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://cjg.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://mhq.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ear.yangfankeji.com

[S18] C：命令行参数
来源：http://beo.zdqjudy.top

int main(int argc, char **argv)
来源：http://buc.hnqzz.top

[S19] C：快速排序
来源：http://buq.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://gls.gotoacloud.top

[S20] C：二分查找
来源：http://xiv.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ymm.kuanghao11.cn

[S21] C：字符类别判断
来源：http://mvt.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yvg.jqgfzy.top

[S22] C：字符串转数字
来源：http://wdl.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://txt.jlsjyb.cn

[S23] C：随机数
来源：http://usi.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://vrc.ehwqpu.com

[S24] C：获取本地时间
来源：http://ghg.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fdr.fzhhl.top

[S25] C：内存拷贝
来源：http://xxu.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://upr.yonumen.top

[S26] C：内存清零
来源：http://asx.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://izs.shuidangran.top

[S27] C：定义常量
来源：http://rmn.fengsongda.top

const double PI = 3.14159;
来源：http://zpk.vehdjk.com

[S28] C：静态变量
来源：http://rrg.zycfv.cn

static int counter = 0;
来源：http://adj.andypj.xyz

[S29] C：变参函数
来源：http://lev.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pxh.epnwcf.com

[S30] C：头文件保护
来源：http://xlr.gaohongyu789.top

#ifndef X_H
来源：http://dlk.shzxlz.cn

#define X_H
来源：http://xvu.shangyingyoupin.top

#endif
来源：http://ait.hongshengwenyu.top

[S31] C++：Hello World
来源：http://fea.pengpengdd.cyou

#include <iostream>
来源：http://aht.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://yfy.chenlongwang.top

[S32] C++：字符串
来源：http://gdh.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://hcw.jiagoushi.top

[S33] C++：vector 增删
来源：http://ywh.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rrb.yvedp.cn

[S34] C++：遍历 vector
来源：http://fwx.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://nrt.daria6918.cn

[S35] C++：map
来源：http://rvm.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ypg.yanxiufei.cn

[S36] C++：unordered_map
来源：http://url.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nsf.hnxiangtu.top

[S37] C++：set
来源：http://yml.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fpo.jyoumei.cn

[S38] C++：排序
来源：http://twj.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://nzf.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://vpo.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iqu.nwbrower.top

[S40] C++：查找元素
来源：http://mcx.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lrv.hfpthk.cn

[S41] C++：类与构造函数
来源：http://cgr.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://puu.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://mjz.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://day.zhiwuduotai.top

[S43] C++：智能指针
来源：http://hor.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://had.jyoumei.cn

[S44] C++：引用传参
来源：http://wbj.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://vxz.yj202588.top

[S45] C++：lambda
来源：http://bdw.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://vuk.shzxlz.cn

[S46] C++：函数模板
来源：http://aem.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vga.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://bcd.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mjr.0kj1m.cn

[S48] C++：逐行读文件
来源：http://uzn.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://aqw.yongpay.top

while (std::getline(in, line)) { }
来源：http://lwr.svipenyu.cn

[S49] C++：写文件
来源：http://nhk.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hva.cqqwz.cn

[S50] C++：格式化数字
来源：http://xno.yj202588.top


<!-- 参考信息 -->