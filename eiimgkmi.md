代发 wailian999

SHOW INDEX FROM users;
来源：http://luu.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://krh.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zkg.guowangkeji.top

[Q74] 强制使用索引
来源：http://uag.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hrm.guowangkeji.top

[Q75] 日期格式化
来源：http://bpx.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vsg.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ioz.mhx1999.top

[Q76] 按天统计
来源：http://aln.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dwa.yuanzhike.top

[Q77] 时间加减
来源：http://sag.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mhw.vehdjk.com

[Q78] 当前时间
来源：http://ogj.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kty.fengsongda.top

[Q79] 字符串拼接
来源：http://dwl.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mds.andypj.xyz

[Q80] 字符串截取
来源：http://xsb.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sye.yj202588.top

[Q81] 字符串替换
来源：http://fqe.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yut.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://yyx.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hmh.hcnkem.com

[Q83] 大小写转换
来源：http://bit.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vag.jianghu66.top

[Q84] 去除首尾空格
来源：http://yfv.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://zyt.hysaishi.cn

[Q85] 数值取整
来源：http://rir.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zkm.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://thc.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jqd.jianghu66.top

[Q87] JSON 字段做条件
来源：http://znh.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qri.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://exu.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mzb.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pop.tanke756.top

[Q89] 判断表是否存在
来源：http://arh.epnwcf.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jam.yonumen.top

[Q90] 生成序号列
来源：http://ixx.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gvn.chenlongwang.top

================================================================================
来源：http://nom.yonumen.top

R. Bash 专题
来源：http://grg.xingfuxueyuan.xyz

================================================================================
来源：http://sjs.zhixingplan.top

[R01] shebang 与严格模式
来源：http://ssx.havefunace.top

#!/usr/bin/env bash
来源：http://yyv.tanke756.top

set -euo pipefail
来源：http://mbv.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://gtn.shzxlz.cn

name="Tom"; echo "$name"
来源：http://rsx.meibo888.top

[R03] 只读变量
来源：http://vxz.jlsjyb.cn

readonly PI=3.14
来源：http://glc.jinqigfzy.top

[R04] 位置参数
来源：http://bqo.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fku.9152youxi.cn

[R05] 参数默认值
来源：http://xqg.yangfankeji.com

name="${1:-default}"
来源：http://mzh.yj202588.top

[R06] 判断命令是否存在
来源：http://jhy.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://olb.yuanzhike.top

[R07] if 判断文件
来源：http://lxm.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://orl.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://gjb.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vtp.haohaochexian.top

[R09] 字符串比较
来源：http://ezu.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssv.yueranfly.top

[R10] 正则匹配
来源：http://svh.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aav.wangdashe.top

[R11] case 多分支
来源：http://cfo.nanxuanxn.top

case "$1" in
来源：http://egb.xuanzx.com

start) echo "启动" ;;
来源：http://tpo.hesvh.cn

stop)  echo "停止" ;;
来源：http://zoh.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://fyp.shzxlz.cn

esac
来源：http://czb.ydjk.org.cn

[R12] for 遍历文件
来源：http://nzq.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://zyf.chenzaomai.com

[R13] for 计数循环
来源：http://suw.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://siw.52xcode.cn

[R14] C 风格 for
来源：http://qvx.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lbe.yanxiufei.cn

[R15] while 逐行读文件
来源：http://gpc.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rkb.tianlin.xyz

[R16] until 等待条件
来源：http://nqe.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qbt.ctjpmb.com

[R17] 数组定义与取值
来源：http://awh.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://gss.guannengcc.top

[R18] 遍历数组
来源：http://nns.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xcu.ybcxt.top

[R19] 数组长度
来源：http://sow.jiagoushi.top

echo "${#arr[@]}"
来源：http://hee.yongpay.top

[R20] 关联数组（字典）
来源：http://koo.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oot.cashguo.top

[R21] 字符串长度
来源：http://hct.yongpay.top

echo "${#s}"
来源：http://uho.hysaishi.cn

[R22] 截取子串
来源：http://gyh.vehdjk.com

echo "${s:0:5}"
来源：http://qpp.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://pzi.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jsk.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://znn.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://vcb.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://xth.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://imv.zhoulong.xyz

[R26] 命令替换
来源：http://xhk.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://jbx.yuxming.cn

[R27] 算术展开
来源：http://etl.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://okk.fktsv.cn

[R28] 浮点运算
来源：http://thr.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://jdw.zhoulong.xyz

[R29] 定义函数
来源：http://ahv.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rlt.jinqigfzy.top

[R30] 函数返回状态码
来源：http://ewd.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://hwy.daxiang520.top

[R31] 局部变量
来源：http://hpn.hesvh.cn

f() { local x=1; echo "$x"; }
来源：http://uyh.yueranfly.top

[R32] 参数个数校验
来源：http://zjd.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ttx.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://nwu.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fxw.fengsongda.top

[R34] 退出时清理
来源：http://sxc.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://nyg.hfpthk.cn

[R35] 后台执行并等待
来源：http://dun.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://icr.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://hcj.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wge.smart0.xyz

[R37] 把输出赋给变量
来源：http://nip.vqdsnc.cn

files=$(ls -1)
来源：http://qvy.ehwqpu.com

[R38] 管道串联
来源：http://oxw.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://jsx.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://ycd.hcnkem.com

cmd > out.log 2>&1
来源：http://zyi.zhoulong.xyz

[R40] 追加写日志
来源：http://iac.xuetiantiany.cn

echo "log" >> out.log
来源：http://njn.yuxming.cn

[R41] 丢弃输出
来源：http://udm.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://rex.zhongyouzk.top

[R42] 输入重定向
来源：http://oyf.zhengqikj.top

wc -l < a.txt
来源：http://kpb.mhx1999.top

[R43] 按名字查找文件
来源：http://ify.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://nvq.hfpthk.cn

[R44] 按修改时间查找
来源：http://dgj.uphjek.com

find . -mtime -7 -type f
来源：http://ylc.ehwqpu.com

[R45] 批量删除
来源：http://ryl.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://asb.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://ttr.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://esh.chenlongwang.top

[R47] sed 单行替换
来源：http://mld.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://guh.yangfankeji.com

[R48] awk 取指定列
来源：http://wvo.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://ujv.aizwys.cn

[R49] awk 带条件
来源：http://ddc.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ewb.ydjk.org.cn

[R50] awk 求和
来源：http://ael.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kgt.jyoumei.cn

[R51] 排序去重取前几
来源：http://okx.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sat.fehbvm.com

[R52] 统计行数
来源：http://qpy.shanyushiyangtech.top

wc -l a.txt
来源：http://ium.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://ddt.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lwt.vehdjk.com

[R54] 比较两个文件
来源：http://nhc.shangyingyoupin.top

diff a.txt b.txt
来源：http://gcb.xinyue.icu

[R55] 压缩与解压
来源：http://akc.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dff.meibo888.top

[R56] 远程拷贝
来源：http://wjo.sweek.top

scp file user@host:/path/
来源：http://rxu.sjlbkw.cn

[R57] 远程执行命令
来源：http://ctq.fktsv.cn

ssh user@host 'uptime'
来源：http://jup.vehdjk.com

[R58] 下载文件
来源：http://vcs.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eyw.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://bie.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ngz.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://gok.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bsw.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://dpm.jyoumei.cn

df -h;  du -sh *
来源：http://rwk.meibo888.top

[R62] 找最占空间的文件
来源：http://mmz.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://fmh.gogol.net.cn

[R63] 内存与进程
来源：http://hct.316326.xyz

free -h;  ps aux | grep nginx
来源：http://swa.daxiang520.top

[R64] 结束进程
来源：http://fgy.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://aoo.tanke756.top

[R65] 查看端口占用
来源：http://trt.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rpk.zhengqikj.top

[R66] 定时任务
来源：http://efi.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://oao.fehbvm.com

[R67] 生成随机十六进制串
来源：http://yms.316326.xyz

openssl rand -hex 16
来源：http://qew.shzxlz.cn

[R68] 计算文件校验值
来源：http://xyp.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://lcl.aibaodan.cn

[R69] 生成随机密码
来源：http://dpd.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://mto.iojbl.cn

[R70] 时间戳与互转
来源：http://oro.guannengcc.top

date +%s;  date -d @1700000000
来源：http://rtd.zhiwuduotai.top

[R71] 日期格式化
来源：http://ibg.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://emo.andypj.xyz

[R72] 等待端口就绪
来源：http://vud.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zyo.ydzc1.top

[R73] 分割大日志
来源：http://ijs.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://hxq.ppjwa.cn

[R74] 批量重命名
来源：http://tsh.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ozc.wangshuangyany.cn

[R75] 导出环境变量
来源：http://wwc.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://wmh.ydzc1.top

[R76] 使用临时文件
来源：http://anx.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ilt.tian-w.cn

[R77] 读取用户输入
来源：http://xqm.52xcode.cn

read -rp "请输入: " ans
来源：http://vqw.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://prg.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qcy.bjfxy.top

[R79] 解析命令行选项
来源：http://mpb.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kkv.cashguo.top

[R80] 查看脚本执行耗时
来源：http://uiz.fengsongda.top

time ./run.sh
来源：http://zhl.yuxming.cn

================================================================================
来源：http://dpy.yueranfly.top

S. C / C++ 专题
来源：http://fdh.yvedp.cn

================================================================================
来源：http://vpb.sjlbkw.cn

[S01] C：Hello World
来源：http://jvl.hongshengwenyu.top

#include <stdio.h>
来源：http://qxa.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://phz.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://gbr.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://lfy.jyoumei.cn

[S03] C：读入整数
来源：http://ybh.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://zis.hnqzz.top

[S04] C：字符串复制
来源：http://uiz.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://ezc.cucudq.cn

[S05] C：字符串长度
来源：http://yox.epnwcf.com

strlen(s)
来源：http://vry.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://wok.guowangkeji.top

strcmp(a, b) == 0
来源：http://fjp.yj20258.top

[S07] C：数组遍历求和
来源：http://sip.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ghz.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://blt.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cil.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://gor.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iqp.tianlin.xyz

[S10] C：指针与解引用
来源：http://ynu.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://nkf.mhx1999.top

[S11] C：逐行读文件
来源：http://ltg.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://vaq.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gyl.dianchejie.cn

fclose(f);
来源：http://spl.jinghuilouyu.cn

[S12] C：写文件
来源：http://kzo.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xwc.yj20258888.top

[S13] C：宏定义
来源：http://hdw.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nmo.jinyuanbaomall.cn

[S14] C：枚举
来源：http://gth.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://eld.bbcook.cn

[S15] C：类型转换
来源：http://kch.gaohongyu789.top

(double) a / b
来源：http://hpq.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://lnh.feifeiyinyue.top

x |= (1 << 3);
来源：http://keg.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://mfv.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sab.sxryk.cn

[S18] C：命令行参数
来源：http://fsk.zdqjudy.top

int main(int argc, char **argv)
来源：http://xbj.9152youxi.cn

[S19] C：快速排序
来源：http://zih.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ket.quarkkingdee.top

[S20] C：二分查找
来源：http://iut.gaohongyu789.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xos.52xcode.cn

[S21] C：字符类别判断
来源：http://kox.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sjl.sufxvd.cn

[S22] C：字符串转数字
来源：http://mtc.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ueg.ehwqpu.com

[S23] C：随机数
来源：http://rkj.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ufm.zhijiandao.cn

[S24] C：获取本地时间
来源：http://xrn.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iks.316326.xyz

[S25] C：内存拷贝
来源：http://goo.tian-w.cn

memcpy(dst, src, n);
来源：http://kxv.zdqjudy.top

[S26] C：内存清零
来源：http://vgc.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://zyb.wangdashe.top

[S27] C：定义常量
来源：http://zjz.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://xra.tanke756.top

[S28] C：静态变量
来源：http://lyh.cashguo.top

static int counter = 0;
来源：http://sii.yanxiufei.cn

[S29] C：变参函数
来源：http://zek.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yne.sysykeji.top

[S30] C：头文件保护
来源：http://aqo.kuanghao11.cn

#ifndef X_H
来源：http://bqh.hnxiangtu.top

#define X_H
来源：http://wey.bjfxy.top

#endif
来源：http://gtt.yj202588.top

[S31] C++：Hello World
来源：http://yzb.svipenyu.cn

#include <iostream>
来源：http://vul.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://xaz.sweek.top

[S32] C++：字符串
来源：http://aub.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://yxq.yvedp.cn

[S33] C++：vector 增删
来源：http://tya.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xmb.uphjek.com

[S34] C++：遍历 vector
来源：http://djj.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://mha.ctjpmb.com

[S35] C++：map
来源：http://edx.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vxh.chenlongwang.top

[S36] C++：unordered_map
来源：http://qov.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vag.chenlongwang.top

[S37] C++：set
来源：http://ubi.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uws.yfazqb.com

[S38] C++：排序
来源：http://tdx.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://cdr.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://vdd.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rbw.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://mga.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nzv.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://tgp.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ggo.vehdjk.com

[S42] C++：继承与虚函数
来源：http://xil.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://sec.meibo888.top


<!-- 参考信息 -->