代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lod.iojbl.cn

[Q54] 清空表
来源：http://sve.c1oappe.top

TRUNCATE TABLE logs;
来源：http://kwx.fengsongda.top

[Q55] 排名（并列占位）
来源：http://btd.cashguo.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://erh.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://mkx.hnxiangtu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wwp.hfpthk.cn

[Q57] 行号
来源：http://rwo.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://crm.snrcjt.cn

[Q58] 累计求和
来源：http://tqd.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bbj.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://rgr.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zwh.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://dgt.cdnleiting.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rod.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ths.shanyushiyangtech.top

[Q61] 移动平均
来源：http://uoe.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rof.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://oct.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qkn.pycfn.com

[Q63] 开启事务
来源：http://gyb.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cpc.meibo888.top

[Q64] 提交事务
来源：http://dgj.aibaodan.cn

COMMIT;
来源：http://nek.hongshengwenyu.top

[Q65] 回滚事务
来源：http://skr.jyoumei.cn

ROLLBACK;
来源：http://xeb.wangshuangyany.cn

[Q66] 行锁查询
来源：http://vti.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rva.snrcjt.cn

[Q67] 设置隔离级别
来源：http://zdj.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cxo.ywan-chungtsiang.top

[Q68] 保存点
来源：http://pdv.zycfv.cn

SAVEPOINT sp1;
来源：http://epf.redwolf501.top

ROLLBACK TO sp1;
来源：http://fzr.yueranfly.top

[Q69] 查看执行计划
来源：http://dzq.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://osj.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://egs.yangfankeji.com

ANALYZE TABLE users;
来源：http://muh.sweek.top

[Q71] 查看建表语句
来源：http://sxf.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blm.yuanzhike.top

[Q72] 查看索引
来源：http://fxr.daxiang520.top

SHOW INDEX FROM users;
来源：http://tvh.yj20258888.top

[Q73] 查看表状态
来源：http://fhg.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wyc.fengsongda.top

[Q74] 强制使用索引
来源：http://acu.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tnf.hnqzz.top

[Q75] 日期格式化
来源：http://xwq.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lgu.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bun.yj202588.top

[Q76] 按天统计
来源：http://ulr.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pna.sxryk.cn

[Q77] 时间加减
来源：http://ael.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zno.ybcxt.top

[Q78] 当前时间
来源：http://cmw.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nei.yj202588.top

[Q79] 字符串拼接
来源：http://qyl.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fqi.jinqigfzy.top

[Q80] 字符串截取
来源：http://nnk.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://heq.zhongyouzk.top

[Q81] 字符串替换
来源：http://knb.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jwe.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://jtd.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ujn.fehbvm.com

[Q83] 大小写转换
来源：http://lil.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xln.sysykeji.top

[Q84] 去除首尾空格
来源：http://cim.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://bai.xylfe.cn

[Q85] 数值取整
来源：http://rjz.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gxg.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://lmn.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xqo.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://lrk.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aey.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://kwy.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bww.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hvk.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://hbz.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tek.yj202588.top

[Q90] 生成序号列
来源：http://tmj.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eys.meibo888.top

================================================================================
来源：http://sak.cqqwz.cn

R. Bash 专题
来源：http://lny.fzhhl.top

================================================================================
来源：http://byl.yvedp.cn

[R01] shebang 与严格模式
来源：http://aix.zhixingplan.top

#!/usr/bin/env bash
来源：http://mkw.aizwys.cn

set -euo pipefail
来源：http://iqo.sweek.top

[R02] 变量赋值与使用
来源：http://jcm.hywenlv.cn

name="Tom"; echo "$name"
来源：http://vip.jqgufenzy.top

[R03] 只读变量
来源：http://nba.havefunace.top

readonly PI=3.14
来源：http://nnm.hysaishi.cn

[R04] 位置参数
来源：http://pme.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://erj.zhoulong.xyz

[R05] 参数默认值
来源：http://ilq.jinqigufen.top

name="${1:-default}"
来源：http://yyt.hfpthk.cn

[R06] 判断命令是否存在
来源：http://rvl.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rqt.quarkkingdee.top

[R07] if 判断文件
来源：http://icu.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tcc.aibaodan.cn

[R08] 数值比较
来源：http://yho.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ghn.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://hfz.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fro.yfazqb.com

[R10] 正则匹配
来源：http://yod.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eti.jiagoushi.top

[R11] case 多分支
来源：http://dkn.havefunace.top

case "$1" in
来源：http://key.hesvh.cn

start) echo "启动" ;;
来源：http://cvo.cdnleiting.top

stop)  echo "停止" ;;
来源：http://pxk.bbcook.cn

*)     echo "未知命令" ;;
来源：http://cfq.yonumen.top

esac
来源：http://fah.jinqigufen.top

[R12] for 遍历文件
来源：http://ilj.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://yep.cdnleiting.top

[R13] for 计数循环
来源：http://kuj.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://zvc.guannengcc.top

[R14] C 风格 for
来源：http://tqx.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fra.hesvh.cn

[R15] while 逐行读文件
来源：http://gvp.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iuw.birdmap.top

[R16] until 等待条件
来源：http://jiq.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vwe.xinyue.icu

[R17] 数组定义与取值
来源：http://fex.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dqs.yuanzhike.top

[R18] 遍历数组
来源：http://bfg.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hxs.yonumen.top

[R19] 数组长度
来源：http://nsu.daxiang520.top

echo "${#arr[@]}"
来源：http://igq.yj20258.top

[R20] 关联数组（字典）
来源：http://afo.svipenyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ejx.feifeiyinyue.top

[R21] 字符串长度
来源：http://fia.shanyushiyangkeji.top

echo "${#s}"
来源：http://tjx.316326.xyz

[R22] 截取子串
来源：http://bel.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://pgr.dashuyun.cn

[R23] 字符串替换
来源：http://ens.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qgs.cucudq.cn

[R24] 大小写转换
来源：http://gry.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ira.andypj.xyz

[R25] 去后缀 / 去前缀
来源：http://ufd.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dxa.52xcode.cn

[R26] 命令替换
来源：http://pwa.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://qrq.vqdsnc.cn

[R27] 算术展开
来源：http://dbs.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://gty.zycfv.cn

[R28] 浮点运算
来源：http://ohx.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://fwb.redwolf501.top

[R29] 定义函数
来源：http://ahe.nwbrower.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://noc.c1oappe.top

[R30] 函数返回状态码
来源：http://foi.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://vnd.sufxvd.cn

[R31] 局部变量
来源：http://oug.sweek.top

f() { local x=1; echo "$x"; }
来源：http://elh.nanxuanxn.top

[R32] 参数个数校验
来源：http://cxf.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jwh.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://ext.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pxy.smart0.xyz

[R34] 退出时清理
来源：http://lgn.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://xze.yangfankeji.com

[R35] 后台执行并等待
来源：http://ici.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vae.daxiang520.top

[R36] 并发执行多个任务
来源：http://sri.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nrn.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://cpi.yanxiufei.cn

files=$(ls -1)
来源：http://hsu.jinyuanbaomall.cn

[R38] 管道串联
来源：http://omv.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://cuq.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://rze.daxiang520.top

cmd > out.log 2>&1
来源：http://ell.yj20258888.top

[R40] 追加写日志
来源：http://qhb.yvedp.cn

echo "log" >> out.log
来源：http://gpf.cdnleiting.top

[R41] 丢弃输出
来源：http://wsd.52xcode.cn

cmd >/dev/null 2>&1
来源：http://kxk.xylfe.cn

[R42] 输入重定向
来源：http://vgt.nanxinkj.top

wc -l < a.txt
来源：http://mim.kuanghao11.cn

[R43] 按名字查找文件
来源：http://ntj.gotoacloud.top

find . -name "*.log" -type f
来源：http://hdn.nanxinkj.top

[R44] 按修改时间查找
来源：http://oie.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://psa.gotoacloud.top

[R45] 批量删除
来源：http://dih.vehdjk.com

find . -name "*.tmp" -delete
来源：http://kfe.hysaishi.cn

[R46] 递归替换文件内容
来源：http://awa.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gag.feifeiyinyue.top

[R47] sed 单行替换
来源：http://sxz.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://ozq.fktsv.cn

[R48] awk 取指定列
来源：http://asc.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://jkz.hysaishi.cn

[R49] awk 带条件
来源：http://sgk.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ldc.jinqigufen.top

[R50] awk 求和
来源：http://zie.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://kvj.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://uct.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vdu.gaohongyu789.top

[R52] 统计行数
来源：http://xjj.gotoacloud.top

wc -l a.txt
来源：http://nsh.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://yaa.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://upe.xziqi.cn

[R54] 比较两个文件
来源：http://tce.tian-w.cn

diff a.txt b.txt
来源：http://bzv.ivvv.top

[R55] 压缩与解压
来源：http://sjw.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jmg.gzhubu.top

[R56] 远程拷贝
来源：http://flc.ybcxt.top

scp file user@host:/path/
来源：http://cnv.feifeiyinyue.top

[R57] 远程执行命令
来源：http://yor.hfpthk.cn

ssh user@host 'uptime'
来源：http://ilf.yvedp.cn

[R58] 下载文件
来源：http://vph.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jxt.zhongyouzk.top

[R59] 发 POST JSON
来源：http://iqs.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://maz.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://wws.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ric.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://xkx.andypj.xyz

df -h;  du -sh *
来源：http://wkk.yvedp.cn

[R62] 找最占空间的文件
来源：http://hkf.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://xdd.chenjidiqi.icu

[R63] 内存与进程
来源：http://yjf.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://lts.aizwys.cn

[R64] 结束进程
来源：http://nmn.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://uqd.yj20258888.top

[R65] 查看端口占用
来源：http://yoo.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rav.pycfn.com

[R66] 定时任务
来源：http://rzc.dashuyun.cn

crontab -e;  crontab -l
来源：http://lht.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://guk.zdbjq.cn

openssl rand -hex 16
来源：http://ojj.nwbrower.top

[R68] 计算文件校验值
来源：http://zei.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://nvk.ybcxt.top

[R69] 生成随机密码
来源：http://utb.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://tde.316326.xyz

[R70] 时间戳与互转
来源：http://rjg.pycfn.com

date +%s;  date -d @1700000000
来源：http://kar.fanxiaobao.xyz

[R71] 日期格式化
来源：http://zkm.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://owg.cucudq.cn

[R72] 等待端口就绪
来源：http://kll.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://axh.hnqzz.top

[R73] 分割大日志
来源：http://hde.svipenyu.cn

split -l 1000 big.log part_
来源：http://cqv.ydjk.org.cn

[R74] 批量重命名
来源：http://uzb.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oea.ehwqpu.com

[R75] 导出环境变量
来源：http://vtp.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://eoh.dashuyun.cn

[R76] 使用临时文件
来源：http://oyv.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ldh.ivvv.top

[R77] 读取用户输入
来源：http://nyl.ctjpmb.com

read -rp "请输入: " ans
来源：http://ryk.gogol.net.cn

[R78] 交互式菜单
来源：http://koz.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ifp.hfpthk.cn

[R79] 解析命令行选项
来源：http://sfs.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lbs.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://any.chenzaomai.com

time ./run.sh
来源：http://izt.jinyuanbaomall.cn

================================================================================
来源：http://ebi.yj20258888.top

S. C / C++ 专题
来源：http://ggp.zhoulong.xyz

================================================================================
来源：http://acr.gzhubu.top

[S01] C：Hello World
来源：http://sgw.hesvh.cn

#include <stdio.h>
来源：http://xvu.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://xcj.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://tav.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://ucn.meibo888.top

[S03] C：读入整数
来源：http://qdz.andypj.xyz

int x; scanf("%d", &x);
来源：http://xkj.ydzc1.top

[S04] C：字符串复制
来源：http://fmy.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://mma.zhongyouzk.top

[S05] C：字符串长度
来源：http://ieu.yuxming.cn

strlen(s)
来源：http://waq.tarul.cn

[S06] C：字符串比较
来源：http://onn.xuetiantiany.cn

strcmp(a, b) == 0
来源：http://kcv.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://owm.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nga.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://eah.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rkp.uphjek.com

[S09] C：结构体定义与初始化
来源：http://rcg.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://epk.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://frx.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://dft.mhx1999.top

[S11] C：逐行读文件
来源：http://dds.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://pqa.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pnq.vehdjk.com

fclose(f);
来源：http://ldz.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://vqd.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fku.yanxiufei.cn

[S13] C：宏定义
来源：http://ufm.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fnc.sysykeji.top

[S14] C：枚举
来源：http://htr.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://cio.kuanghao11.cn

[S15] C：类型转换
来源：http://bhk.uphjek.com

(double) a / b
来源：http://ucu.yj202588.top

[S16] C：位操作置位
来源：http://rfn.jianghu66.top

x |= (1 << 3);
来源：http://iib.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://bbs.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rng.yueranfly.top

[S18] C：命令行参数
来源：http://mfe.hysaishi.cn

int main(int argc, char **argv)
来源：http://nqr.quarkkingdee.top

[S19] C：快速排序
来源：http://yqk.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://anv.tian-w.cn

[S20] C：二分查找
来源：http://gmf.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bwd.ehwqpu.com

[S21] C：字符类别判断
来源：http://ybf.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://she.kuanghao11.cn

[S22] C：字符串转数字
来源：http://blw.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://nzb.jyoumei.cn

[S23] C：随机数
来源：http://sdx.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jzm.gogol.net.cn

[S24] C：获取本地时间
来源：http://uxu.redwolf501.top


<!-- 参考信息 -->