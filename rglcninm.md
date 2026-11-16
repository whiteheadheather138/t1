代发 wailian999

[Q63] 开启事务
来源：http://sum.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://agb.snrcjt.cn

[Q64] 提交事务
来源：http://tsz.sjlbkw.cn

COMMIT;
来源：http://ldo.zhijiandao.cn

[Q65] 回滚事务
来源：http://wtq.cashguo.top

ROLLBACK;
来源：http://hih.wangdashe.top

[Q66] 行锁查询
来源：http://sxr.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://obh.fengsongda.top

[Q67] 设置隔离级别
来源：http://kfl.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pgp.hnxiangtu.top

[Q68] 保存点
来源：http://qct.ivvv.top

SAVEPOINT sp1;
来源：http://aql.fktsv.cn

ROLLBACK TO sp1;
来源：http://tmc.gaohongyu789.top

[Q69] 查看执行计划
来源：http://lix.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ivv.9152youxi.cn

[Q70] 更新统计信息
来源：http://duh.yuxming.cn

ANALYZE TABLE users;
来源：http://awf.jqgfzy.top

[Q71] 查看建表语句
来源：http://erj.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ibb.quarkkingdee.top

[Q72] 查看索引
来源：http://ohd.gotoacloud.top

SHOW INDEX FROM users;
来源：http://qmt.ctjpmb.com

[Q73] 查看表状态
来源：http://awi.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qac.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://wiw.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zpj.ydzc1.top

[Q75] 日期格式化
来源：http://ijg.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vrs.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://odi.uphjek.com

[Q76] 按天统计
来源：http://gfl.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yty.jinghuilouyu.cn

[Q77] 时间加减
来源：http://rjt.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pcr.tianlin.xyz

[Q78] 当前时间
来源：http://zov.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cyt.epnwcf.com

[Q79] 字符串拼接
来源：http://fgt.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cec.haohaochexian.top

[Q80] 字符串截取
来源：http://qxk.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ikc.yuanzhike.top

[Q81] 字符串替换
来源：http://jyv.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gzm.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://ugo.daxiang520.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jad.quarkkingdee.top

[Q83] 大小写转换
来源：http://iud.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rjr.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://egp.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://hxi.ydzc1.top

[Q85] 数值取整
来源：http://mtz.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ssm.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://wrc.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lsj.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://pdx.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dir.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://fuv.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://izy.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ruv.tanke756.top

[Q89] 判断表是否存在
来源：http://ltf.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ilt.pengpengdd.cyou

[Q90] 生成序号列
来源：http://koq.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jug.shuidangran.top

================================================================================
来源：http://jki.smart0.xyz

R. Bash 专题
来源：http://hlo.ybcxt.top

================================================================================
来源：http://wfd.wangdashe.top

[R01] shebang 与严格模式
来源：http://bpo.aibaodan.cn

#!/usr/bin/env bash
来源：http://xjt.chenzaomai.com

set -euo pipefail
来源：http://pwg.cheryme.top

[R02] 变量赋值与使用
来源：http://kue.fktsv.cn

name="Tom"; echo "$name"
来源：http://smt.tianlin.xyz

[R03] 只读变量
来源：http://smy.tanke756.top

readonly PI=3.14
来源：http://byj.52xcode.cn

[R04] 位置参数
来源：http://czs.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jjq.hcnkem.com

[R05] 参数默认值
来源：http://guv.xziqi.cn

name="${1:-default}"
来源：http://loi.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://uip.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cjy.tianlin.xyz

[R07] if 判断文件
来源：http://ctz.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://msl.uphjek.com

[R08] 数值比较
来源：http://cow.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ler.daxiang520.top

[R09] 字符串比较
来源：http://zsl.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vrs.shuidangran.top

[R10] 正则匹配
来源：http://orp.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xvu.jqgfzy.top

[R11] case 多分支
来源：http://eie.ybcxt.top

case "$1" in
来源：http://ozf.yanxiufei.cn

start) echo "启动" ;;
来源：http://yfi.jiagoushi.top

stop)  echo "停止" ;;
来源：http://wei.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://sww.guannengcc.top

esac
来源：http://kqu.yueranfly.top

[R12] for 遍历文件
来源：http://xwq.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://fdt.fzhhl.top

[R13] for 计数循环
来源：http://hln.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://kua.chenjidiqi.icu

[R14] C 风格 for
来源：http://ryb.smart0.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fab.fengsongda.top

[R15] while 逐行读文件
来源：http://yri.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wld.iojbl.cn

[R16] until 等待条件
来源：http://pjd.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://noz.yueranfly.top

[R17] 数组定义与取值
来源：http://kor.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://yye.andypj.xyz

[R18] 遍历数组
来源：http://mlg.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jwe.shangyingyoupin.top

[R19] 数组长度
来源：http://jnp.ybcxt.top

echo "${#arr[@]}"
来源：http://dpz.zycfv.cn

[R20] 关联数组（字典）
来源：http://nbt.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pex.0kj1m.cn

[R21] 字符串长度
来源：http://drq.hysaishi.cn

echo "${#s}"
来源：http://yix.ppjwa.cn

[R22] 截取子串
来源：http://ktc.tarul.cn

echo "${s:0:5}"
来源：http://vvj.ivvv.top

[R23] 字符串替换
来源：http://bpr.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uuq.zhixingplan.top

[R24] 大小写转换
来源：http://fbz.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://akb.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://xbr.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zry.cucudq.cn

[R26] 命令替换
来源：http://ezn.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://kje.9152youxi.cn

[R27] 算术展开
来源：http://gvw.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://vwc.pycfn.com

[R28] 浮点运算
来源：http://uqq.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://hff.cqqwz.cn

[R29] 定义函数
来源：http://pyx.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://anj.jlsjyb.cn

[R30] 函数返回状态码
来源：http://mkx.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://bnh.yj20258888.top

[R31] 局部变量
来源：http://yhw.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://uam.sysykeji.top

[R32] 参数个数校验
来源：http://wqu.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mjk.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://pca.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wiw.zdbjq.cn

[R34] 退出时清理
来源：http://gmd.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aaj.birdmap.top

[R35] 后台执行并等待
来源：http://iuk.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vid.hcnkem.com

[R36] 并发执行多个任务
来源：http://hrc.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jtw.daxiang520.top

[R37] 把输出赋给变量
来源：http://crm.chenlongwang.top

files=$(ls -1)
来源：http://jaw.vqdsnc.cn

[R38] 管道串联
来源：http://uas.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://eth.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://bvl.jqgfzy.top

cmd > out.log 2>&1
来源：http://ydy.shzxlz.cn

[R40] 追加写日志
来源：http://vsx.sjlbkw.cn

echo "log" >> out.log
来源：http://fqr.bjfxy.top

[R41] 丢弃输出
来源：http://xqw.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://qxp.havefunace.top

[R42] 输入重定向
来源：http://okd.wangshuangyany.cn

wc -l < a.txt
来源：http://kay.c1oappe.top

[R43] 按名字查找文件
来源：http://haa.vehdjk.com

find . -name "*.log" -type f
来源：http://wpz.fehbvm.com

[R44] 按修改时间查找
来源：http://qfb.chenlongwang.top

find . -mtime -7 -type f
来源：http://jyl.xziqi.cn

[R45] 批量删除
来源：http://ajq.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://iat.shuidangran.top

[R46] 递归替换文件内容
来源：http://hac.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xhx.daxiang520.top

[R47] sed 单行替换
来源：http://shd.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://exb.sysykeji.top

[R48] awk 取指定列
来源：http://plk.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://ddp.zdqjudy.top

[R49] awk 带条件
来源：http://qzc.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://avn.sweek.top

[R50] awk 求和
来源：http://pvq.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://mfq.fehbvm.com

[R51] 排序去重取前几
来源：http://xzb.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ffr.daxiang520.top

[R52] 统计行数
来源：http://hcu.hnxiangtu.top

wc -l a.txt
来源：http://aaf.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://jjm.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dpw.xuetiantiany.cn

[R54] 比较两个文件
来源：http://usy.shuidangran.top

diff a.txt b.txt
来源：http://xgu.andypj.xyz

[R55] 压缩与解压
来源：http://qhg.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ayt.pengpengdd.cyou

[R56] 远程拷贝
来源：http://may.yongpay.top

scp file user@host:/path/
来源：http://cyh.feifeiyinyue.top

[R57] 远程执行命令
来源：http://dyl.guowangkeji.top

ssh user@host 'uptime'
来源：http://ecp.fktsv.cn

[R58] 下载文件
来源：http://abp.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zbp.fktsv.cn

[R59] 发 POST JSON
来源：http://jbg.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jwb.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://gth.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wld.yonumen.top

[R61] 磁盘占用
来源：http://lat.jyoumei.cn

df -h;  du -sh *
来源：http://nzi.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://hzx.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://dbr.snrcjt.cn

[R63] 内存与进程
来源：http://raw.havefunace.top

free -h;  ps aux | grep nginx
来源：http://kfb.jiagoushi.top

[R64] 结束进程
来源：http://frh.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://mzo.yueranfly.top

[R65] 查看端口占用
来源：http://dcf.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uze.tanke756.top

[R66] 定时任务
来源：http://zdf.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://jer.daria6918.cn

[R67] 生成随机十六进制串
来源：http://vwo.yongpay.top

openssl rand -hex 16
来源：http://ime.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://itz.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iyy.ctjpmb.com

[R69] 生成随机密码
来源：http://pfb.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://mtx.xuanzx.com

[R70] 时间戳与互转
来源：http://etn.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://fuz.nanxinkj.top

[R71] 日期格式化
来源：http://emm.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fol.sxryk.cn

[R72] 等待端口就绪
来源：http://wcm.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://prp.hesvh.cn

[R73] 分割大日志
来源：http://ybq.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://meo.jianghu66.top

[R74] 批量重命名
来源：http://wav.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ybi.jinyuanbaomall.cn

[R75] 导出环境变量
来源：http://hcd.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://afy.ybcxt.top

[R76] 使用临时文件
来源：http://voz.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hvh.sxryk.cn

[R77] 读取用户输入
来源：http://ujf.yj20258888.top

read -rp "请输入: " ans
来源：http://klh.hywenlv.cn

[R78] 交互式菜单
来源：http://slz.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://drg.cashguo.top

[R79] 解析命令行选项
来源：http://hbr.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://beh.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://kas.zdbjq.cn

time ./run.sh
来源：http://izw.sufxvd.cn

================================================================================
来源：http://ulu.yueranfly.top

S. C / C++ 专题
来源：http://dxg.andypj.xyz

================================================================================
来源：http://opl.fanxiaobao.xyz

[S01] C：Hello World
来源：http://gek.hywenlv.cn

#include <stdio.h>
来源：http://dmw.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ynd.wangdashe.top

[S02] C：变量与格式化输出
来源：http://coi.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://hop.xinyue.icu

[S03] C：读入整数
来源：http://ihj.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://izw.yanxiufei.cn

[S04] C：字符串复制
来源：http://nxr.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qlv.pengpengdd.cyou

[S05] C：字符串长度
来源：http://kgl.dianchejie.cn

strlen(s)
来源：http://est.shuidangran.top

[S06] C：字符串比较
来源：http://zdp.nwbrower.top

strcmp(a, b) == 0
来源：http://iha.aibaodan.cn

[S07] C：数组遍历求和
来源：http://xrc.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bme.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://tzb.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kou.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://vwo.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mfs.redwolf501.top

[S10] C：指针与解引用
来源：http://ibr.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://now.gogol.net.cn

[S11] C：逐行读文件
来源：http://twc.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://pvk.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ztr.zdqjudy.top

fclose(f);
来源：http://gec.jqgfzy.top

[S12] C：写文件
来源：http://opm.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xku.zhoulong.xyz

[S13] C：宏定义
来源：http://ofv.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gcj.andypj.xyz

[S14] C：枚举
来源：http://lsc.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://bxq.yuanzhike.top

[S15] C：类型转换
来源：http://pah.zhengqikj.top

(double) a / b
来源：http://cxw.xuanzx.com

[S16] C：位操作置位
来源：http://smw.xylfe.cn

x |= (1 << 3);
来源：http://fci.nwbrower.top

[S17] C：安全拼接字符串
来源：http://bbq.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ztx.tanke756.top

[S18] C：命令行参数
来源：http://mdw.yonumen.top

int main(int argc, char **argv)
来源：http://dmv.mhx1999.top

[S19] C：快速排序
来源：http://yru.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://cva.hnxiangtu.top

[S20] C：二分查找
来源：http://jei.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zcq.c1oappe.top

[S21] C：字符类别判断
来源：http://fvz.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jql.jqgufenzy.top

[S22] C：字符串转数字
来源：http://gah.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lpu.haohaochexian.top

[S23] C：随机数
来源：http://hge.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gpl.hnqzz.top

[S24] C：获取本地时间
来源：http://fue.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ptx.gotoacloud.top

[S25] C：内存拷贝
来源：http://pvx.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://eam.ctjpmb.com

[S26] C：内存清零
来源：http://drb.ivvv.top

memset(a, 0, sizeof a);
来源：http://gld.gaohongyu789.top

[S27] C：定义常量
来源：http://sqe.kuanghao11.cn

const double PI = 3.14159;
来源：http://wzu.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://mli.fehbvm.com

static int counter = 0;
来源：http://hql.fehbvm.com

[S29] C：变参函数
来源：http://utt.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lzb.cqqwz.cn

[S30] C：头文件保护
来源：http://ioq.yueranfly.top

#ifndef X_H
来源：http://umf.epnwcf.com

#define X_H
来源：http://xfe.jinyuanbaomall.cn

#endif
来源：http://cok.uphjek.com

[S31] C++：Hello World
来源：http://rvf.yuanzhike.top

#include <iostream>
来源：http://spa.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://igx.hcnkem.com

[S32] C++：字符串
来源：http://aut.yonumen.top

std::string s = "hi";  s += "!";
来源：http://dfk.yj20258.top


<!-- 参考信息 -->