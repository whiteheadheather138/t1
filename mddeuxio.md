代发 wailian999

SHOW INDEX FROM users;
来源：http://mnw.yj20258.top

[Q73] 查看表状态
来源：http://eyd.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://obb.xingfuxueyuan.xyz

[Q74] 强制使用索引
来源：http://qkw.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wxo.wangshuangyany.cn

[Q75] 日期格式化
来源：http://nye.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yfk.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kdv.ydjk.org.cn

[Q76] 按天统计
来源：http://yce.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hkl.ivvv.top

[Q77] 时间加减
来源：http://qwb.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vpu.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://psf.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://skh.svipenyu.cn

[Q79] 字符串拼接
来源：http://jlr.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ogj.yangfankeji.com

[Q80] 字符串截取
来源：http://jzv.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kws.fengsongda.top

[Q81] 字符串替换
来源：http://xdp.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://msu.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://wmw.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://djw.daria6918.cn

[Q83] 大小写转换
来源：http://mml.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bxd.iojbl.cn

[Q84] 去除首尾空格
来源：http://tft.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://ogj.hywenlv.cn

[Q85] 数值取整
来源：http://pde.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jsx.tarul.cn

[Q86] 读取 JSON 字段
来源：http://myc.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ylo.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://owa.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://smu.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://uvu.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mey.zhongyouzk.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://urf.shzxlz.cn

[Q89] 判断表是否存在
来源：http://mtv.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vqy.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://crt.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://law.yongpay.top

================================================================================
来源：http://lnv.kuanghao11.cn

R. Bash 专题
来源：http://cjg.jlsjyb.cn

================================================================================
来源：http://wcb.xinyue.icu

[R01] shebang 与严格模式
来源：http://jnb.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://oyb.nwbrower.top

set -euo pipefail
来源：http://cba.tarul.cn

[R02] 变量赋值与使用
来源：http://xzy.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://yci.zhoulong.xyz

[R03] 只读变量
来源：http://agz.yueranfly.top

readonly PI=3.14
来源：http://hpk.hywenlv.cn

[R04] 位置参数
来源：http://aei.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://khq.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://pug.chenjidiqi.icu

name="${1:-default}"
来源：http://isk.316326.xyz

[R06] 判断命令是否存在
来源：http://ioa.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cbs.ivvv.top

[R07] if 判断文件
来源：http://tik.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://grg.ppjwa.cn

[R08] 数值比较
来源：http://axn.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jpn.ydzc1.top

[R09] 字符串比较
来源：http://dke.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xxx.wangshuangyany.cn

[R10] 正则匹配
来源：http://ude.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://egi.birdmap.top

[R11] case 多分支
来源：http://gob.shuidangran.top

case "$1" in
来源：http://xps.redwolf501.top

start) echo "启动" ;;
来源：http://ijc.yj202588.top

stop)  echo "停止" ;;
来源：http://ykl.c1oappe.top

*)     echo "未知命令" ;;
来源：http://dvs.zhixingplan.top

esac
来源：http://klo.cdnleiting.top

[R12] for 遍历文件
来源：http://stu.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://yrv.hongshengwenyu.top

[R13] for 计数循环
来源：http://vkn.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://cmh.yuxming.cn

[R14] C 风格 for
来源：http://ofs.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jwa.sjlbkw.cn

[R15] while 逐行读文件
来源：http://nja.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wom.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://wvv.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ccn.yueranfly.top

[R17] 数组定义与取值
来源：http://kdn.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lhn.guowangkeji.top

[R18] 遍历数组
来源：http://min.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://clz.ppjwa.cn

[R19] 数组长度
来源：http://qth.tian-w.cn

echo "${#arr[@]}"
来源：http://bye.svipenyu.cn

[R20] 关联数组（字典）
来源：http://jkh.fktsv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gqw.chenjidiqi.icu

[R21] 字符串长度
来源：http://egi.zhengqikj.top

echo "${#s}"
来源：http://wla.yangfankeji.com

[R22] 截取子串
来源：http://eki.fengsongda.top

echo "${s:0:5}"
来源：http://wnn.sufxvd.cn

[R23] 字符串替换
来源：http://wnn.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lvm.jiagoushi.top

[R24] 大小写转换
来源：http://mxx.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nzj.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://oqp.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://uoe.shanyushiyangtech.top

[R26] 命令替换
来源：http://npm.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://gti.hcnkem.com

[R27] 算术展开
来源：http://gxu.sxryk.cn

echo $((1 + 2 * 3))
来源：http://qbn.shzxlz.cn

[R28] 浮点运算
来源：http://biq.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://vvc.snrcjt.cn

[R29] 定义函数
来源：http://bzj.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dnf.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://yxt.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://pdr.vqdsnc.cn

[R31] 局部变量
来源：http://gwc.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://xou.yj202588.top

[R32] 参数个数校验
来源：http://vsw.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tvz.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://hor.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fto.daxiang520.top

[R34] 退出时清理
来源：http://jzp.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://kbe.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://zzo.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://vvt.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://riv.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nif.vehdjk.com

[R37] 把输出赋给变量
来源：http://tcd.sysykeji.top

files=$(ls -1)
来源：http://sqp.feifeiyinyue.top

[R38] 管道串联
来源：http://yta.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://jgc.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://xet.birdmap.top

cmd > out.log 2>&1
来源：http://gml.tianlin.xyz

[R40] 追加写日志
来源：http://ipp.hfpthk.cn

echo "log" >> out.log
来源：http://frf.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://dzf.havefunace.top

cmd >/dev/null 2>&1
来源：http://rte.bjfxy.top

[R42] 输入重定向
来源：http://uar.feifeiyinyue.top

wc -l < a.txt
来源：http://gcb.hnxiangtu.top

[R43] 按名字查找文件
来源：http://ixy.cucudq.cn

find . -name "*.log" -type f
来源：http://riu.redwolf501.top

[R44] 按修改时间查找
来源：http://rcq.ybcxt.top

find . -mtime -7 -type f
来源：http://puk.yfazqb.com

[R45] 批量删除
来源：http://fqf.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://evt.c1oappe.top

[R46] 递归替换文件内容
来源：http://los.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tbf.guannengcc.top

[R47] sed 单行替换
来源：http://dmq.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://dtn.quarkkingdee.top

[R48] awk 取指定列
来源：http://lyf.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://ube.jianghu66.top

[R49] awk 带条件
来源：http://rqr.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wxt.sxryk.cn

[R50] awk 求和
来源：http://mwt.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bux.ydzc1.top

[R51] 排序去重取前几
来源：http://ydd.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://acp.jlsjyb.cn

[R52] 统计行数
来源：http://yos.hnqzz.top

wc -l a.txt
来源：http://lqx.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://pdw.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dgy.uphjek.com

[R54] 比较两个文件
来源：http://kdh.jlsjyb.cn

diff a.txt b.txt
来源：http://hjc.tanke756.top

[R55] 压缩与解压
来源：http://nbo.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cms.c1oappe.top

[R56] 远程拷贝
来源：http://kqs.shzxlz.cn

scp file user@host:/path/
来源：http://gfq.cqqwz.cn

[R57] 远程执行命令
来源：http://dsy.hnxiangtu.top

ssh user@host 'uptime'
来源：http://xpw.jiagoushi.top

[R58] 下载文件
来源：http://dqv.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fvh.jqgufenzy.top

[R59] 发 POST JSON
来源：http://mws.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vov.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://dyg.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kwj.yj20258888.top

[R61] 磁盘占用
来源：http://qfp.zhengqikj.top

df -h;  du -sh *
来源：http://icc.daxiang520.top

[R62] 找最占空间的文件
来源：http://mmp.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://mhm.fehbvm.com

[R63] 内存与进程
来源：http://gll.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://kfo.fktsv.cn

[R64] 结束进程
来源：http://mvo.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://jwy.quarkkingdee.top

[R65] 查看端口占用
来源：http://fjb.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wou.gaohongyu789.top

[R66] 定时任务
来源：http://dob.chenzaomai.com

crontab -e;  crontab -l
来源：http://mhe.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://zqo.jyoumei.cn

openssl rand -hex 16
来源：http://rrb.birdmap.top

[R68] 计算文件校验值
来源：http://qom.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hry.andypj.xyz

[R69] 生成随机密码
来源：http://qeb.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://nqi.pycfn.com

[R70] 时间戳与互转
来源：http://lsk.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://skn.zhengqikj.top

[R71] 日期格式化
来源：http://xbl.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sbu.yj20258888.top

[R72] 等待端口就绪
来源：http://wwz.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ffe.guannengcc.top

[R73] 分割大日志
来源：http://pju.daria6918.cn

split -l 1000 big.log part_
来源：http://tbi.yanxiufei.cn

[R74] 批量重命名
来源：http://nks.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jjj.mhx1999.top

[R75] 导出环境变量
来源：http://hyd.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://mbp.sjlbkw.cn

[R76] 使用临时文件
来源：http://pno.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uhs.nanxuanxn.top

[R77] 读取用户输入
来源：http://vef.svipenyu.cn

read -rp "请输入: " ans
来源：http://omz.zhijiandao.cn

[R78] 交互式菜单
来源：http://jwg.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tff.c1oappe.top

[R79] 解析命令行选项
来源：http://iqz.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://moe.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://qks.dianchejie.cn

time ./run.sh
来源：http://gku.fzhhl.top

================================================================================
来源：http://jad.gotoacloud.top

S. C / C++ 专题
来源：http://goq.yanxiufei.cn

================================================================================
来源：http://wec.epnwcf.com

[S01] C：Hello World
来源：http://byo.ivvv.top

#include <stdio.h>
来源：http://lxk.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vum.yj20258.top

[S02] C：变量与格式化输出
来源：http://njf.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://jgi.zdqjudy.top

[S03] C：读入整数
来源：http://asj.jinqigufen.top

int x; scanf("%d", &x);
来源：http://dak.yonumen.top

[S04] C：字符串复制
来源：http://mcz.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://azv.hywenlv.cn

[S05] C：字符串长度
来源：http://kzf.xingfuxueyuan.xyz

strlen(s)
来源：http://pyq.chenjidiqi.icu

[S06] C：字符串比较
来源：http://gql.hfpthk.cn

strcmp(a, b) == 0
来源：http://ret.redwolf501.top

[S07] C：数组遍历求和
来源：http://elj.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sxn.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://pcs.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wob.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://dfj.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qkq.daria6918.cn

[S10] C：指针与解引用
来源：http://dfe.bbcook.cn

int *p = &a;  *p = 5;
来源：http://wuv.tanke756.top

[S11] C：逐行读文件
来源：http://qjy.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://hxs.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://bie.tianlin.xyz

fclose(f);
来源：http://ryp.jlsjyb.cn

[S12] C：写文件
来源：http://qcr.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lds.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://vcy.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hdm.andypj.xyz

[S14] C：枚举
来源：http://rcs.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://opp.jinghuilouyu.cn

[S15] C：类型转换
来源：http://ojb.pengpengdd.cyou

(double) a / b
来源：http://wqc.chenzaomai.com

[S16] C：位操作置位
来源：http://orw.daria6918.cn

x |= (1 << 3);
来源：http://nvy.vehdjk.com

[S17] C：安全拼接字符串
来源：http://yta.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mti.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://jnj.svipenyu.cn

int main(int argc, char **argv)
来源：http://oyv.hnqzz.top

[S19] C：快速排序
来源：http://kqi.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://mmm.pengpengdd.cyou

[S20] C：二分查找
来源：http://njl.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cds.cashguo.top

[S21] C：字符类别判断
来源：http://zfb.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wlc.ehwqpu.com

[S22] C：字符串转数字
来源：http://eob.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hew.zhoulong.xyz

[S23] C：随机数
来源：http://fwq.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qlv.316326.xyz

[S24] C：获取本地时间
来源：http://jqu.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://maq.52xcode.cn

[S25] C：内存拷贝
来源：http://wto.zhixingplan.top

memcpy(dst, src, n);
来源：http://kgv.iojbl.cn

[S26] C：内存清零
来源：http://eek.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://mon.feifeiyinyue.top

[S27] C：定义常量
来源：http://ecv.vehdjk.com

const double PI = 3.14159;
来源：http://hoa.jinqigfzy.top

[S28] C：静态变量
来源：http://jha.ydjk.org.cn

static int counter = 0;
来源：http://tao.gogol.net.cn

[S29] C：变参函数
来源：http://yak.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://msi.zdqjudy.top

[S30] C：头文件保护
来源：http://ozg.zdbjq.cn

#ifndef X_H
来源：http://qmh.redwolf501.top

#define X_H
来源：http://utj.gzhubu.top

#endif
来源：http://jsb.redwolf501.top

[S31] C++：Hello World
来源：http://xde.guowangkeji.top

#include <iostream>
来源：http://tzn.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://hlu.ivvv.top

[S32] C++：字符串
来源：http://wzq.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://xyk.daria6918.cn

[S33] C++：vector 增删
来源：http://vex.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://upj.tianlin.xyz

[S34] C++：遍历 vector
来源：http://jmz.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://hxm.quarkkingdee.top

[S35] C++：map
来源：http://luh.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kbb.jlsjyb.cn

[S36] C++：unordered_map
来源：http://vob.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://feg.jqgfzy.top

[S37] C++：set
来源：http://ubs.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jfg.jinqigfzy.top

[S38] C++：排序
来源：http://ysw.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://ncl.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://eve.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bpi.c1oappe.top

[S40] C++：查找元素
来源：http://kam.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wbp.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://juc.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hdu.yj202588.top

[S42] C++：继承与虚函数
来源：http://syw.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://xek.fzhhl.top


<!-- 参考信息 -->