代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gqo.zhijiandao.cn

[Q50] 批量更新
来源：http://uxs.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://flk.hywenlv.cn

[Q51] 用子查询更新
来源：http://mws.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xii.jinqigfzy.top

[Q52] 删除指定行
来源：http://rhh.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://ezs.zhengqikj.top

[Q53] 按条件删除
来源：http://hzy.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jns.nanxinkj.top

[Q54] 清空表
来源：http://gwo.nanxinkj.top

TRUNCATE TABLE logs;
来源：http://tpr.hesvh.cn

[Q55] 排名（并列占位）
来源：http://ogp.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ixb.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://mnh.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://por.52xcode.cn

[Q57] 行号
来源：http://xcn.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://spz.ydzc1.top

[Q58] 累计求和
来源：http://ysn.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ood.daxiang520.top

[Q59] 分组内累计
来源：http://cjf.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mhd.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://spl.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wkg.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jqx.wangdashe.top

[Q61] 移动平均
来源：http://ozp.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ysk.tarul.cn

[Q62] 分组占比
来源：http://jxu.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gcy.shzxlz.cn

[Q63] 开启事务
来源：http://tgy.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hmq.feifeiyinyue.top

[Q64] 提交事务
来源：http://djb.sxryk.cn

COMMIT;
来源：http://oft.nwbrower.top

[Q65] 回滚事务
来源：http://omx.jlsjyb.cn

ROLLBACK;
来源：http://gcj.andypj.xyz

[Q66] 行锁查询
来源：http://wbq.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rxo.aizwys.cn

[Q67] 设置隔离级别
来源：http://vdw.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gth.sjlbkw.cn

[Q68] 保存点
来源：http://ymn.redwolf501.top

SAVEPOINT sp1;
来源：http://kua.shuidangran.top

ROLLBACK TO sp1;
来源：http://zna.jinqigfzy.top

[Q69] 查看执行计划
来源：http://jfe.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://etx.bbcook.cn

[Q70] 更新统计信息
来源：http://hsn.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://cnm.fzhhl.top

[Q71] 查看建表语句
来源：http://utk.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cym.andypj.xyz

[Q72] 查看索引
来源：http://boj.ehwqpu.com

SHOW INDEX FROM users;
来源：http://bgp.yonumen.top

[Q73] 查看表状态
来源：http://eob.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bjf.yfazqb.com

[Q74] 强制使用索引
来源：http://gld.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://orw.iojbl.cn

[Q75] 日期格式化
来源：http://bbx.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rsq.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ntg.chenlongwang.top

[Q76] 按天统计
来源：http://sch.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bwy.jlsjyb.cn

[Q77] 时间加减
来源：http://rdh.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wjb.yfazqb.com

[Q78] 当前时间
来源：http://gvv.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hte.c1oappe.top

[Q79] 字符串拼接
来源：http://dcx.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://crr.ydjk.org.cn

[Q80] 字符串截取
来源：http://zvr.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xju.jinqigufen.top

[Q81] 字符串替换
来源：http://dmn.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hfz.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://ate.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zyv.smart0.xyz

[Q83] 大小写转换
来源：http://zhk.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fzn.0kj1m.cn

[Q84] 去除首尾空格
来源：http://vfk.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://hph.meibo888.top

[Q85] 数值取整
来源：http://vju.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kse.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://whs.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dux.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://osi.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://agv.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://ytq.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xeb.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yct.zhixingplan.top

[Q89] 判断表是否存在
来源：http://brx.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xzp.sjlbkw.cn

[Q90] 生成序号列
来源：http://wtc.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rzl.hnqzz.top

================================================================================
来源：http://dyw.xingfuxueyuan.xyz

R. Bash 专题
来源：http://zch.ydjk.org.cn

================================================================================
来源：http://vif.chenzaomai.com

[R01] shebang 与严格模式
来源：http://qqz.yangfankeji.com

#!/usr/bin/env bash
来源：http://gam.yangfankeji.com

set -euo pipefail
来源：http://aga.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://klo.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://axi.jqgfzy.top

[R03] 只读变量
来源：http://zgx.vehdjk.com

readonly PI=3.14
来源：http://qqu.andypj.xyz

[R04] 位置参数
来源：http://kyc.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vej.ehwqpu.com

[R05] 参数默认值
来源：http://isv.cashguo.top

name="${1:-default}"
来源：http://sho.xziqi.cn

[R06] 判断命令是否存在
来源：http://dpg.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zhk.hnxiangtu.top

[R07] if 判断文件
来源：http://amy.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rqt.sweek.top

[R08] 数值比较
来源：http://ugv.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://dwc.epnwcf.com

[R09] 字符串比较
来源：http://vup.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oiu.yangfankeji.com

[R10] 正则匹配
来源：http://yvv.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xmo.hnxiangtu.top

[R11] case 多分支
来源：http://hna.xuanzx.com

case "$1" in
来源：http://ndb.0kj1m.cn

start) echo "启动" ;;
来源：http://ahr.9152youxi.cn

stop)  echo "停止" ;;
来源：http://ysl.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://ysr.meibo888.top

esac
来源：http://ttv.yueranfly.top

[R12] for 遍历文件
来源：http://fvr.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://njl.birdmap.top

[R13] for 计数循环
来源：http://ybb.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://dcz.fengsongda.top

[R14] C 风格 for
来源：http://fty.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nju.kuanghao11.cn

[R15] while 逐行读文件
来源：http://yyu.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rde.zhixingplan.top

[R16] until 等待条件
来源：http://tgx.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nep.cqqwz.cn

[R17] 数组定义与取值
来源：http://guq.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://qeg.yongpay.top

[R18] 遍历数组
来源：http://mbk.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://omi.chenlongwang.top

[R19] 数组长度
来源：http://qjd.zhoulong.xyz

echo "${#arr[@]}"
来源：http://wrp.snrcjt.cn

[R20] 关联数组（字典）
来源：http://sac.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mpi.zdqjudy.top

[R21] 字符串长度
来源：http://wpc.shuidangran.top

echo "${#s}"
来源：http://skb.jinghuilouyu.cn

[R22] 截取子串
来源：http://mge.yj202588.top

echo "${s:0:5}"
来源：http://qos.daxiang520.top

[R23] 字符串替换
来源：http://drg.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dnn.yvedp.cn

[R24] 大小写转换
来源：http://ujo.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://ufh.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://bqj.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oml.yuxming.cn

[R26] 命令替换
来源：http://qwo.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://fnd.cqqwz.cn

[R27] 算术展开
来源：http://hwo.dianchejie.cn

echo $((1 + 2 * 3))
来源：http://vek.smart0.xyz

[R28] 浮点运算
来源：http://vst.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://lcg.jyoumei.cn

[R29] 定义函数
来源：http://dcy.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ngl.gzhubu.top

[R30] 函数返回状态码
来源：http://jde.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://zbu.gogol.net.cn

[R31] 局部变量
来源：http://fbk.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://qgs.zhongyouzk.top

[R32] 参数个数校验
来源：http://lls.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vok.uphjek.com

[R33] 捕获错误并提示行号
来源：http://zts.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rjw.meibo888.top

[R34] 退出时清理
来源：http://fjd.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://akx.bbcook.cn

[R35] 后台执行并等待
来源：http://rme.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://idj.nanxinkj.top

[R36] 并发执行多个任务
来源：http://mrg.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hfh.jyoumei.cn

[R37] 把输出赋给变量
来源：http://xer.pengpengdd.cyou

files=$(ls -1)
来源：http://moc.jinghuilouyu.cn

[R38] 管道串联
来源：http://ndx.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://dvw.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://xhr.cheryme.top

cmd > out.log 2>&1
来源：http://ixf.hfpthk.cn

[R40] 追加写日志
来源：http://imc.hysaishi.cn

echo "log" >> out.log
来源：http://lfh.yvedp.cn

[R41] 丢弃输出
来源：http://env.ybcxt.top

cmd >/dev/null 2>&1
来源：http://mid.ydzc1.top

[R42] 输入重定向
来源：http://tpt.fzhhl.top

wc -l < a.txt
来源：http://beu.zhixingplan.top

[R43] 按名字查找文件
来源：http://sio.gaohongyu789.top

find . -name "*.log" -type f
来源：http://coc.hysaishi.cn

[R44] 按修改时间查找
来源：http://nyf.ydzc1.top

find . -mtime -7 -type f
来源：http://yqy.shanyushiyangkeji.top

[R45] 批量删除
来源：http://vua.yonumen.top

find . -name "*.tmp" -delete
来源：http://yey.cucudq.cn

[R46] 递归替换文件内容
来源：http://tox.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mzu.cashguo.top

[R47] sed 单行替换
来源：http://odg.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://qnj.jyoumei.cn

[R48] awk 取指定列
来源：http://qit.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://tcz.bbcook.cn

[R49] awk 带条件
来源：http://nre.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ukz.fengsongda.top

[R50] awk 求和
来源：http://mrq.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://kgw.sufxvd.cn

[R51] 排序去重取前几
来源：http://eip.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mlv.ehwqpu.com

[R52] 统计行数
来源：http://jjb.hnqzz.top

wc -l a.txt
来源：http://ncc.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://sfx.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ckz.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://mxq.c1oappe.top

diff a.txt b.txt
来源：http://ehn.jinqigfzy.top

[R55] 压缩与解压
来源：http://vil.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tji.hnxiangtu.top

[R56] 远程拷贝
来源：http://igp.cashguo.top

scp file user@host:/path/
来源：http://oox.c1oappe.top

[R57] 远程执行命令
来源：http://wol.zhixingplan.top

ssh user@host 'uptime'
来源：http://wfh.zdqjudy.top

[R58] 下载文件
来源：http://ujb.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kam.xylfe.cn

[R59] 发 POST JSON
来源：http://sfz.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qsq.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://sqz.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qoq.daria6918.cn

[R61] 磁盘占用
来源：http://erg.jiagoushi.top

df -h;  du -sh *
来源：http://mtl.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://zeh.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://jbi.ybcxt.top

[R63] 内存与进程
来源：http://tax.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://qpe.shangyingyoupin.top

[R64] 结束进程
来源：http://mvw.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://mil.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://ckp.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dqn.ehwqpu.com

[R66] 定时任务
来源：http://hjl.xuanzx.com

crontab -e;  crontab -l
来源：http://whl.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://mfy.zdbjq.cn

openssl rand -hex 16
来源：http://wzp.bbcook.cn

[R68] 计算文件校验值
来源：http://rer.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://twn.cashguo.top

[R69] 生成随机密码
来源：http://ndg.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://cwa.yonumen.top

[R70] 时间戳与互转
来源：http://jmk.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://sjv.tanke756.top

[R71] 日期格式化
来源：http://voe.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ttp.tarul.cn

[R72] 等待端口就绪
来源：http://mvz.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://psw.iojbl.cn

[R73] 分割大日志
来源：http://cie.xylfe.cn

split -l 1000 big.log part_
来源：http://hkg.aibaodan.cn

[R74] 批量重命名
来源：http://mgv.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sje.uphjek.com

[R75] 导出环境变量
来源：http://uir.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://wzo.pengpengdd.cyou

[R76] 使用临时文件
来源：http://qgs.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gmp.vqdsnc.cn

[R77] 读取用户输入
来源：http://kra.tianlin.xyz

read -rp "请输入: " ans
来源：http://kag.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://qbl.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yvl.shuidangran.top

[R79] 解析命令行选项
来源：http://cwj.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pqd.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://lya.shuidangran.top

time ./run.sh
来源：http://pel.yvedp.cn

================================================================================
来源：http://tlh.52xcode.cn

S. C / C++ 专题
来源：http://kve.gogol.net.cn

================================================================================
来源：http://nyl.svipenyu.cn

[S01] C：Hello World
来源：http://kvw.sufxvd.cn

#include <stdio.h>
来源：http://vhw.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lim.yueranfly.top

[S02] C：变量与格式化输出
来源：http://kgm.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://sli.hcnkem.com

[S03] C：读入整数
来源：http://jet.svipenyu.cn

int x; scanf("%d", &x);
来源：http://tfp.pengpengdd.cyou

[S04] C：字符串复制
来源：http://lna.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://gat.chenlongwang.top

[S05] C：字符串长度
来源：http://qmr.cashguo.top

strlen(s)
来源：http://hjw.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://wmg.hesvh.cn

strcmp(a, b) == 0
来源：http://nmf.uphjek.com

[S07] C：数组遍历求和
来源：http://bqc.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hdq.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://kfh.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wtp.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://ioo.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pin.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://sah.yuxming.cn

int *p = &a;  *p = 5;
来源：http://jey.snrcjt.cn

[S11] C：逐行读文件
来源：http://xzf.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://zsu.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uou.gotoacloud.top

fclose(f);
来源：http://gjj.sweek.top

[S12] C：写文件
来源：http://rqr.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hwq.yueranfly.top

[S13] C：宏定义
来源：http://ojm.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gld.snrcjt.cn

[S14] C：枚举
来源：http://den.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://pnv.sweek.top

[S15] C：类型转换
来源：http://yld.cheryme.top

(double) a / b
来源：http://cgv.kuanghao11.cn

[S16] C：位操作置位
来源：http://atj.aibaodan.cn

x |= (1 << 3);
来源：http://sed.shuidangran.top

[S17] C：安全拼接字符串
来源：http://cni.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qmz.zhijiandao.cn

[S18] C：命令行参数
来源：http://wqj.tian-w.cn

int main(int argc, char **argv)
来源：http://gkw.andypj.xyz

[S19] C：快速排序
来源：http://yqo.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://xbn.fengsongda.top

[S20] C：二分查找
来源：http://ops.daxiang520.top


<!-- 参考信息 -->